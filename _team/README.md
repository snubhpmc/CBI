# Team Members

이 폴더에서 팀원 정보를 관리합니다.

## 새 팀원 추가 방법

1. 새 마크다운 파일 생성 (예: `john-doe.md`)
2. Front matter 작성:

```markdown
---
name: John Doe
role: PhD Student  # Principal Investigator, Postdoc, PhD Student, Master Student
position: PhD candidate
year: 2024-present
email: john@example.com
photo: john.jpg  # assets/img/team/ 폴더에 사진 저장
google_scholar: https://scholar.google.com/...
order: 20  # 작을수록 먼저 표시 (PI=1, PhD=10~, MS=20~)
research: Deep learning, Genomics
---

## Research Interests
- 관심 분야 1
- 관심 분야 2

## Education
- Ph.D. in ...
- M.S. in ...

## Publications
(자동으로 가져오거나 직접 작성)
```

## Order 가이드
- PI: 1-9
- Postdoc: 10-19
- PhD: 20-49
- Master: 50-79
- Undergraduate: 80-99
- Alumni: 100+
