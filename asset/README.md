# 프로젝트별 공개 이미지 폴더

프로젝트 상세페이지 이미지는 이 폴더에 업로드하면 자동으로 표시됩니다.
파일을 추가하거나 삭제한 뒤 GitHub Pages가 배포되면 사이트가 GitHub 저장소를 읽어 이미지를 갱신합니다.

## 이미지 업로드 방법

1. 아래 프로젝트 ID와 같은 폴더를 엽니다.
2. **Add file → Upload files**를 누릅니다.
3. JPG, JPEG, PNG, WEBP, GIF, AVIF 이미지를 업로드하고 Commit changes를 누릅니다.
4. 사이트에서 해당 프로젝트 상세페이지를 새로고침합니다.

파일명은 자유롭게 정할 수 있습니다. 여러 장이면 파일명 순서(예: 01-cover.webp, 02-plan.webp, 03-section.webp)로 표시됩니다.

## 프로젝트 폴더

| 프로젝트 | 폴더 경로 |
|---|---|
| ON THE LOOPS | `asset/on-the-loops/` |
| SQUARE-RANDE VOUS | `asset/square-rande-vous/` |
| CANYON PARK | `asset/canyon-park/` |
| 추억은 방울방울 | `asset/memories/` |
| WATER MELON HOUSE | `asset/water-melon-house/` |
| 구로동 오피스텔 인테리어 | `asset/guro-officetel/` |

예시:
`asset/on-the-loops/01-cover.webp`

## 표시 방식

- 프로젝트 목록은 각 폴더의 `project.json`(제목, 연도, 위치 등)으로 만들어집니다.
- `project.json`의 `type`은 `ACADEMIC` 또는 `OFFICE`이고, 목록은 타입별로 나뉘어 `order` 값이 작은 순서로 표시됩니다. 관리자 모드에서 카드를 드래그하면 같은 타입 안에서 `order`가 바뀌어 저장됩니다. `project.json`이 없는 폴더는 사이트에 나타나지 않습니다.
- 폴더에 이미지가 한 장 이상 있으면 해당 폴더 이미지들이 상세페이지에 표시됩니다.
- 폴더가 비어 있으면 이미지 없이 빈 썸네일과 안내 문구가 표시됩니다.
- 프로젝트 목록 썸네일도 해당 폴더의 첫 번째 이미지로 자동 변경됩니다.
- 방문자는 읽기만 가능하며, GitHub에 업로드한 공개 파일은 누구나 볼 수 있습니다.
- 관리자 메뉴에서 GitHub 토큰을 입력하면 Add project와 Add images가 이 폴더에 바로 저장됩니다. 토큰이 없으면 해당 기기의 브라우저에만 저장됩니다.

## 관리자 메뉴에서 바로 추가하기

1. 사이트 주소 뒤에 `?manage`를 붙여 열고 **MANAGE**를 누릅니다.
2. **+ Add project**로 프로젝트를 만들면 GitHub 토큰을 묻습니다. 이 저장소의 **Contents: Read and write** 권한만 준 fine-grained Personal Access Token을 입력합니다. 토큰은 그 브라우저에만 저장됩니다.
3. 프로젝트는 `asset/{프로젝트ID}/project.json` 파일로 저장되고, 모든 방문자의 목록에 나타납니다.
4. 프로젝트 상세페이지의 **+ Add images**로 올린 이미지는 `asset/{프로젝트ID}/` 폴더에 커밋됩니다.
5. **Delete project**는 `asset/{프로젝트ID}/` 폴더를 이미지까지 통째로 지웁니다. 되돌리려면 Git 기록에서 복구해야 합니다.
