# Resources

이 폴더에서 연구실의 오픈소스 도구, 데이터셋, 저장소를 관리합니다.

## 새 리소스 추가 방법

1. 새 마크다운 파일 생성 (예: `new-tool.md`)
2. Front matter 작성:

```markdown
---
name: Tool Name
category: Software  # Software, Database, Dataset 등
url: https://github.com/username/repo
order: 10  # 작을수록 먼저 표시
---

도구에 대한 설명을 여기에 작성합니다.
```

## Category 목록
- Software: 소프트웨어 도구
- Database: 데이터베이스
- Dataset: 데이터셋
- Tutorial: 튜토리얼/문서

## 사용 예시

페이지에서:
```liquid
{% assign resources = site.resources | sort: "order" %}
{% for resource in resources %}
  {{ resource.name }} - {{ resource.category }}
  {{ resource.content }}
{% endfor %}
```
