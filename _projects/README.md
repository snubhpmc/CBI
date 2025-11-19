# Research Projects

이 폴더에서 연구 프로젝트를 관리합니다.

## 새 프로젝트 추가 방법

1. 새 마크다운 파일 생성 (예: `new-project.md`)
2. Front matter 작성:

```markdown
---
title: Project Title
category: Multi-Omics Analysis  # 또는 Computational Method Development, Network Biology, Database Resources
description: 짧은 설명
image: project-image.png  # assets/img/research/ 폴더에 이미지 저장
highlight: true  # 홈페이지에 강조 표시 여부
order: 10  # 카테고리 내 순서 (작을수록 먼저 표시)
paper_title: "Related Paper Title"
paper_link: "https://..."
---

프로젝트 상세 설명을 여기에 작성합니다.
마크다운 문법 사용 가능합니다.

## Methods
...

## Results
...
```

## Category 목록
- Multi-Omics Analysis (order: 1-9)
- Computational Method Development (order: 10-19)
- Network Biology (order: 30-39)
- Database Resources (order: 40-49)

## 이미지 없는 프로젝트
image 필드를 비워두면 자동으로 빈 공간으로 표시됩니다.
