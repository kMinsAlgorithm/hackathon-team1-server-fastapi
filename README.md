본 프로젝트는 고객의 질문 정보를 기반으로 적합한 보험 정보를 추천해주는 웹서비스를 구현하는 프로젝트입니다.
### 다국어 질문을 통한 보험 추천 웹 서비스

#### 프로젝트 개요

이 프로젝트는 고객의 질문 정보를 기반으로 적합한 보험 정보를 추천해주는 웹 서비스를 구현하는 것을 목표로 합니다. 고급 자연어 처리(NLP) 기술을 활용하여 다국어 질문을 영어로 번역하고, BERT 기반 명명된 엔티티 인식(NER) 모델을 사용하여 핵심 단어를 추출한 후, 이 단어들을 데이터베이스 내의 관련 보험 상품과 매칭합니다. 이러한 혁신적인 접근 방식은 개별적인 요구와 질문에 맞춤화된 정확하고 문맥을 고려한 보험 추천을 가능하게 합니다.

#### 프로젝트 플로우

1. **다국어 질문을 영어로 번역**
    - NER 모델이 영어 데이터를 기반으로 학습되었기 때문에, 다양한 언어로 된 질문을 영어로 번역하는 것이 중요합니다. 이 단계는 NER 모델이 질문을 정확하게 처리하고 이해할 수 있게 하여, 전 세계 사용자가 서비스를 이용할 수 있게 합니다.

2. **BERT 기반 NER 모델을 사용한 핵심 단어 추출**
    - 이 과정의 핵심은 BERT 기반 NER 모델을 사용하여 영어로 번역된 질문에서 중요한 단어를 식별하고 추출하는 것입니다. 질문의 문맥과 구체적인 세부 사항을 이해함으로써, 모델은 관련 보험 상품과 매칭하기 위해 필수적인 요소들을 정확히 찾아냅니다.

3. **추출된 단어를 기반으로 한 보험 추천**
    - 질문에서 추출된 핵심 단어를 사용하여, 서비스는 보험 정보 데이터베이스를 검색하여 식별된 단어와 높은 연관성을 가진 보험 상품을 찾아냅니다. 이 방법은 사용자의 요구와 밀접하게 연결된 추천을 보장하여, 개인 맞춤형 보험 선택 과정을 제공합니다.

#### 프로젝트의 영향

이 웹 서비스는 고객이 보험 상품을 찾는 방식을 혁신적으로 변화시켜, 검색 과정을 더 효율적이고 정확하며 개인의 요구에 맞춤화될 수 있게 합니다. 복잡한 보험 데이터베이스와 고객의 요구 사이의 간격을 고급 NLP 기술을 통해 연결함으로써, 보험 정보에 대한 원활하고 사용자 친화적인 접근을 제공합니다.


## 🔒 How to start
uvicorn main:app --reload

#### 커밋 컨벤션
예시) `feat: todo 등록 구현`

| 머릿말   | 설명                               |
| -------- | ---------------------------------- |
| feat     | 기능 구현                          |
| setting  | 패키지 설치, 개발 설정             |
| refactor | 기능변화 없이 최적화, 코드 개선 등 |
| fix      | 버그 수정                          |
| style    | 스타일링, 변수명 수정              |
| docs     | README.md 작성,주석 추가           |

#### 브랜치 네이밍 컨벤션

예시) `feature/signIn`

모든 feature는 develop에서 분기합니다

| 머릿말  | 설명                        |
| ------- | --------------------------- |
| master  | 최종 결과                   |
| develop | 기능 구현                   |
| feature | 기능 단위 구현              |
| fix     | master에서 발견된 버그 수정 |

## 🛠 Tech Stack
- FastApi

## api 문서 확인
- http://127.0.0.1:8000/redoc
