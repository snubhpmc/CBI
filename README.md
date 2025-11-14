


## 📝 데이터 업데이트 방법

코드를 수정할 필요 없이 아래 파일들만 편집하면 웹사이트가 자동으로 업데이트됩니다.  

웹사이트의 모든 주요 데이터는 `_data/` 폴더의 YAML 파일에서 관리됩니다.

* research.yml  

```
    # category 
    - category: "Multi-Omics Analysis" 
        category_ko: "" 
        description: "We utilize genomic data to develop personalized treatment strategies and improve patient outcomes through precision medicine approaches."
        keywords: "WGS, WES, RNA-seq, Single-Cell, Spatial Transcriptomics"
        order: 1

        # project 내용
        projects: 
            - title: "Microsatellite Instability Analysis"
                description: "MSI analysis across cancer types for precision oncology"
                image: "DNA-msi.png"
                detail_description: "Comprehensive microsatellite instability (MSI) analysis across various cancer types to identify potential biomarkers for precision oncology and personalized treatment strategies."
                paper_title: ""
                paper_link: ""
                highlight: true #home 페이지 게시여부

```

* team_members.yml  

```
    phd_students:
    - name: "Jin-Ok Lee"
        name_en: "Jin-Ok Lee"
        position: "PhD candidate"
        year: "2022-present"
        email: "jinoklee.01@gmail.com"
        photo: "jolee.jpg"
        google_scholar: "https://scholar.google.com/citations?user=egJ93-4AAAAJ&hl=ko"
        research: "Bioinformatics, Deep learning"

```


논문 리스트는 `_bibliopraphy/` 폴더의 papers.bib 파일에서 관리됩니다.   


```
    @article{cortes2017molecular,
    title={A molecular portrait of microsatellite instability across multiple cancers},
    author={Cortes-Ciriano, Isidro and Lee, Sejoon and Park, Woong-Yang and Kim, Tae-Min and Park, Peter J},
    journal={Nature communications},
    volume={8},
    number={1},
    pages={15180},
    year={2017},
    url={https://www.nature.com/articles/ncomms15180},
    publisher={Nature Publishing Group UK London},
    pmid={28585546}
    }

```




