[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/03H_UnPI)
# Dialogue Summarization | 일상 대화 요약
## Team(NLP_4조)

## 0. Overview
### Environment

- Ubuntu 20.04
- python
- Geforce RTX3090 24GB
- wandb


### Requirements
- _Write Requirements_

## 1. Competiton Info

### Overview

- 경진대회 주제
    - 일상 대화를 요약하는 모델 생성

### Timeline

- May 13, 2024 - Start Date
- May 27, 2024 - Final submission deadline

## 2. Components

### Directory

- _Insert your directory structure_

e.g.
```
├── code
│   ├── jupyter_notebooks
│   │   └── model_train.ipynb
│   └── train.py
├── docs
│   ├── pdf
│   │   └── (Template) [패스트캠퍼스] Upstage AI Lab 1기_그룹 스터디 .pptx
│   └── paper
└── input
    └── data
        ├── eval
        └── train
```

## 3. Data descrption

### Dataset overview
![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/f358f5ce-f403-4d87-b8b3-546ebaaf53be)


### EDA


![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/255ae3de-a896-4e65-8a0f-2abbc91f5a65)


- 본 대회에서는 ROUGE-1-F1, ROUGE-2-F1, ROUGE-L-F1, 총 3가지 종류의 metric으로부터 산출된 평균 점수를 더하여 최종 점수를 계산
- ROUGE는 텍스트 요약, 기계 번역과 같은 태스크를 평가하기 위해 사용되는 대표적인 metric 모델 요약본 혹은 번역본을 사람이 만든 참조 요약본과 비교해 점수를 계산



![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/854b49aa-255e-4b0e-9f19-cd4fff37afc3)

- 토크나이저를 사용해 프롬프트 시퀸스 길이를 확인
    - 평균 시퀀스 길이: 283.8
    - 중앙값 시퀀스 길이: 263.0
    - 최대 시퀀스 길이: 1395
    - 최소 시퀀스 길이: 59
 
![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/63add4e0-e10d-44e1-8e4f-201ac9781006)


- 주요 대화 주제
    - 대부분의 대화가 일상에서 일어나는 주제
    - 비즈니스 대화, 직업 면접 등 비즈니스 상황에서 일어나는 대화도 존재





### Data Processing

- Data Augmentation
![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/9462acea-b042-4dad-93e3-52df77fbfdf2)


![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/b681ad99-58ad-479d-87c1-1cc0b934275a)


![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/d251cc3c-c3e4-4bf4-a09c-16d7916fe042)


![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/4625168c-ed65-4226-af0f-7d3026b8d2cb)





## 4. Modeling

### Model descrition

![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/9862ec58-c919-4eff-8dec-f9216606553e)


### Modeling Process

![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/4f8ddd34-b5e5-4dc2-a26c-f8ffe55c5864)

![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/2706687b-4319-4e5e-a416-49a559bd7536)

![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/b6ae5710-c171-4b2c-ba66-95cf9d150b10)


![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/c60c22c2-7007-4ae3-a263-b0e4a3ef889c)


![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/30e07d1b-8f4e-4479-bb1b-d645d588e374)

![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/64d9445d-bffc-4408-ad94-06a9cdcd6321)


## 5. Result


### Leader Board

![image](https://github.com/UpstageAILab2/upstage-nlp-summarization-nlp-04/assets/114049128/7b493fff-c9ca-4cb9-9ef0-7ec677fc168f)


### Presentation

- _Insert your presentaion file(pdf) link_

## etc

### Meeting Log

- 매일 일정 시간 마다 모여서 회의

### Reference

- _Insert related reference_
