# '카카오톡 대규모 업데이트'는 정말 실패했을까?
### 외부 데이터(VOC) 기반 사용자 피드백 심층 분석 및 개선 전략 제언
카카오톡 v25.8.0 업데이트에 대한 사용자 반응 분석 프로젝트 (구글 스토어, 뉴스, 블로그)

**2025.11.19 ~ 2025.12.13 (Personal Project)**

---

## 1. 프로젝트 요약 (Executive Summary)

해당 프로젝트는 2025년 9월 23일 진행된 카카오톡 v25.8.0 업데이트에 대한 시장의 반응을 **데이터를 통해 입체적으로 분석**하고, "이번 업데이트는 정말 실패했는가?"라는 질문에 답하기 위해 시작되었습니다.

구글 플레이 스토어 리뷰, 네이버 뉴스, 블로그를 통해 **총 16만여 건의 비정형 텍스트 데이터**를 수집 및 분석하여, 사용자들의 핵심 불만 원인을 규명하고, 시간에 따른 여론의 변화 과정을 추적했습니다.

분석 결과, 이번 업데이트는 단순한 UI 변경 문제를 넘어 '**사용자 주권(User Sovereignty) 침해**'라는 근본적인 신뢰의 문제였음을 발견했으며, 이를 바탕으로 **데이터 분석가이자 예비 PM의 관점**에서 구체적인 단기/중장기 개선 전략을 제안합니다.

<br>

> ### **최종 결과물 바로가기**
> *   **[PORTFOLIO]** **[핵심 요약 포트폴리오 (PDF) 보기](./2025_Data_Analysis_Portfolio.pdf)** `<- 클릭!`
> *   **[FULL REPORT]** **[상세 분석 보고서 전체 보기 ([Notion/Blog Link](https://growthpm.tistory.com/6))]** `<- 클릭!` *(분석의 모든 과정과 인사이트를 담았습니다.)*

<br>

---

## 2. 핵심 발견 (Key Findings) & 시각화

|   Finding   | 핵심 내용 | 
|  :---  | :--- |
| **Finding 1** | **분노의 '양'은 줄었지만, '질'은 변하지 않았다.**<br>시간이 흐르며 리뷰의 절대적인 양은 감소했으나, 남아있는 목소리의 부정 감성 비율과 핵심 불만 키워드는 꾸준히 유지되었습니다. |
| **Finding 2** | **모든 불만의 중심에는 '친구 탭'과 '개편 행위'가 있었다.**<br>네트워크 분석 결과, 모든 부정 키워드는 '친구'와 '개편'을 중심으로 하나의 거대한 클러스터를 형성하여, 문제가 총체적이었음을 증명했습니다. |
| **Finding 3** | **사용자, 언론, 블로그는 각기 다른 관점과 역할을 수행했다.**<br>사용자는 '감정'을, 언론은 '시장 영향'을, 블로그는 '해결책'을 이야기하며, 같은 사안을 두고 서로 다른 목소리를 냈습니다. |

<br>

---

## 3. 기술 스택 (Tech Stack)

*   **Data Collection:** `Python`, `Selenium`, `BeautifulSoup4`, `google-play-scraper`
*   **Data Processing & Analysis:** `Python`, `Pandas`, `NumPy`, `Konlpy(Okt)`
*   **NLP & Sentiment Analysis:** `Transformers`, `Hugging Face (matthewburke/korean_sentiment)`
*   **Data Visualization:** `Matplotlib`, `Seaborn`, `WordCloud`, `NetworkX`, `pyLDAvis`
*   **Environment:** `Jupyter Notebook`, `Google Colab`

---

## 4. 프로젝트 구조

이 저장소는 다음과 같은 구조로 이루어져 있습니다.

*   `1_Data_Collection/`: 데이터 수집을 위한 스크립트 모음
*   `2_Data_Preprocessing/`: 수집된 데이터를 분석 가능한 형태로 정제하는 스크립트 모음
*   `3_Deep_Dive_Analysis/`: 핵심 심층 분석을 수행하는 통합 파이프라인 스크립트
*   `Image/`: README 및 보고서에 사용된 핵심 시각화 이미지
*   `Sample_Data/`: 분석에 사용된 데이터의 일부 샘플
*   `2025_Data_Analysis_Portfolio.pdf`: 최종 요약 포트폴리오
*   `Kakao_Final_Report.pdf`: 상세 분석 보고서 PDF 버전

---
