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

- 폴더에 이미지가 한 장 이상 있으면 해당 폴더 이미지들이 상세페이지에 표시됩니다.
- 폴더가 비어 있으면 이미지 없이 빈 썸네일과 안내 문구가 표시됩니다.
- 프로젝트 목록 썸네일도 해당 폴더의 첫 번째 이미지로 자동 변경됩니다.
- 방문자는 읽기만 가능하며, GitHub에 업로드한 공개 파일은 누구나 볼 수 있습니다.
- 브라우저 안의 기존 Add images는 이 기기에만 저장되는 로컬 기능입니다. 전체 방문자에게 공개할 이미지는 반드시 GitHub의 `asset` 폴더에 올려야 합니다.
