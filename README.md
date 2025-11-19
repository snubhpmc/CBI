
# Lab-page 

랩 홈페이지 주소입니다. 

https://snubhpmc.github.io/CBI/

<hr>



## 📝 데이터 업데이트 방법

! 코드를 수정할 필요 없이 아래 파일들만 편집하면 웹사이트가 자동으로 업데이트됩니다.  


HOME페이지의 lab goal 내용은 `_pages/` 폴더의 lab.md 에서 관리합니다. 
```
    Our lab is dedicated to transforming healthcare through data-driven approaches. Our research embodies true disciplinary convergence, integrating Engineering, Biology, and Medicine. By combining clinical data, genomics, and artificial intelligence, we advance precision medicine and improve patient outcomes.

    **Our primary goal** is to support clinicians in molecular diagnosis and treatment decision-making, addressing every stage of the computational pipeline—from initial discovery to clinical translation.

    We integrate clinical and genomic data to identify disease-associated molecular alterations and discover clinically significant biomarkers. These findings guide therapeutic selection through target gene-drug associations and inform the development of practical diagnostic platforms for real-world clinical use.

```


웹사이트의 모든 주요 데이터는 해당 

* _project  

```
    checkmate.md 파일 
    ---
    title: NGS-based Sample Identity Verification
    category: Computational Method Development
    description: Sample identity verification in human using NGS data
    image: checkmate.png
    highlight: false
    order: 12
    ---

    NGS-based sample identity verification tool for human samples to ensure data integrity and prevent sample mix-ups in genomic studies.


```

* _team

```
    jinok-lee.md 파일 
    ---
    name: Jin-Ok Lee
    role: PhD Student
    position: PhD candidate
    year: 2022-present
    email: jinoklee.01@gmail.com
    photo: jolee.jpg
    google_scholar: https://scholar.google.com/citations?user=egJ93-4AAAAJ&hl=ko
    order: 10
    research: Bioinformatics, Deep learning
    ---


```

* _new

```
    2023-12-01.md
    ---
    layout: post
    date: 2023-12-01
    inline: true
    related_posts: false
    title: "Research Grant Awarded"
    ---

    We received funding for STR in healthcare research project.



```





논문 리스트는 `_bibliopraphy/` 폴더의 papers.bib 파일에서 관리합니다.   


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

이미지는 `assets/img` 폴더안에 넣습니다. 
```
    research 폴더 : research 관련 이미지
    team 폴더 : 팀원 사진 

```



