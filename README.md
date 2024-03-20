# The Origin of Korean Cuisine (English ver.)

This is the project data upload repository for the Introduction to Digital Humanities II, Class 05, College of Liberal Arts, Korea University.

## Overview

- This project is part of the Introduction to Digital Humanities II course in the College of Liberal Arts at Korea University.
- The goal is to learn how to use digital humanities tools and deepen understanding in this area.
- We collect data on Korean ingredients and cooking methods from the early modern to modern periods to explore what defines the style of Korean cuisine.
- This project was inspired by [this study](https://www.nature.com/articles/srep00196), but our research focuses more on exploring the unique characteristics of Korean cuisine rather than finding universal food pairing traits.
- The cookbooks we will collect during the fall semester are as follows. These cookbooks are of high documentary value and some are already digitized, making them easily accessible:
  - Sangayorok (산가요록)
  - Eumsik Dimibang (음식디미방)
  - Suun Japbang (수운잡방)
- The list of cookbooks for future reference is excerpted from the book "Food Classics" by Professor Han Bok-ryeo. Please refer to the [Copyright](#copyright) section below if any copyright issues arise.

  ### Cookbooks from the 1400s to 1500s

  - Sangayorok, Suun Japbang, Gyemi Seo

  ### Cookbooks from the 1600s to 1700s

  - Domundaejak, Choissi Eumsikbeop, Singanguhwangchalyo, Eumsik Dimibang, Yorok, Jubangmun, Eumsikbo, Somin Sasul, Jeungbo Sanrim Gyeongje

  ### Cookbooks from the 1800s

  - Gyuhap Chongseo, Imwon Gyeongjeji, Dongguk Sesigi, Yunssi Eumsikbeop, Eumsikbangmun, Gagi Hanjung Ilwol, Eumsikbangmunira, Gyugon Yoram, Jusik Siui, Issi Eumsikbeop, Siui Jeonseo

  ### Cookbooks from the 1900s

  - Banchan Deungsok, Buin Pilji, Joseon Musang Shinsik Yorijebeop, Joseon Yorijebeop, Haedong Jukji, Ganpyeon Joseon Yorijebeop, Sacheui Joseon Yori, Joseon Yoribeop, Gajeong Jubu Pildok, Joseon Yorihak, Uri Eumsik, Ijo Gungjeong Yoritonggo

## How to Contribute to the Project

Everyone who wishes to contribute to the project data is welcome to start contributing after the end of the fall semester.

This project aims to improve students' abilities to use Git/Github, so please contribute in the following ways:

- If you are not familiar with Git or Github, you can learn the basics by referring to [this guide](https://git-scm.com/book/ko/v2).
- When contributing on Github, you can do so through Pull Requests, referring to [the Pull Request guide](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

### How to Contribute Data

1. Download the `template.json` file and read the description for each field thoroughly. Below is an example of the file:

   ```json
   {
     "student_id": "Student ID, Name, Nickname (Please use consistently)",
     "name": "Name of the dish",
     "image": "images/your_image_name.png (Please store the image file in the images folder. JPG format is also acceptable.)",
     "image_prompt": "Prompt used for AI image generation",
     "ingredients": ["Ingredient1", "Ingredient2", "Ingredient3"],
     "original": "Enter the original cooking method here.",
     "translated": "Enter the translation of the cooking method here.",
     "source": "Enter the source of the cooking method here.",
     "comment": "Enter any personal thoughts about this dish or information you want to share with others here."
   }

#### Detailed Instructions for Data Contribution

- **Student ID (`student_id`)**: Please use a string only. This will be used as the file name when uploading. If an ID already exists, a sequential number will be assigned.
- **Dish Name (`name`)**: You must enter the name of a Korean dish, not personal names.
- **Image (`image`)**: Upload the AI-generated Korean dish image to the `images` folder, and the file name must start with `images/`.
- **Prompt (`image_prompt`)**: Specify the prompt used for AI image generation. Perfect reproduction is impossible, but it helps in achieving similar results.
- **Ingredients (`ingredients`)**

  - **Basic Rules**: The list should be submitted in list format, and should not include quantities or cooking status.

    | Input Example       | Description                                   |
    | --------------------| --------------------------------------------- |
    | Not Allowed: 4-5 bushels of beans | Do not specify quantity. Use 'beans'         |
    | Not Allowed: Boiled radish        | Do not specify cooking status. Use 'radish'  |
    | Allowed: Kimchi                   | In recipes like kimchi stew, use 'kimchi'    |

- **Original (`original`)**: Enter the original recipe here. This will be used for data modification and verification.
- **Translation (`translated`)**: If in Classical Chinese or old Korean, provide a translation. Perfect translation is not required as the project mainly aims to verify the use of ingredients.
- **Source (`source`)**: Enter the name of the source book. Write in Korean only, but Hanja (Chinese characters) may be included.
- **Comment (`comment`)**: Enter any notable specifics worth mentioning.

#### Contribution Procedure

1. Copy the `template.json` to the `data` folder and rename it as desired.
2. Upload the AI-generated image to the `images` folder. Avoid duplicating file names.
3. Commit with a freeform message.
4. Create a Pull Request (PR) with the title "Student ID - Dish Name".
5. Wait for PR approval. The format will be verified by an automatic script. If rejected, check the message, make corrections, and retry.

## Data Visualization

The results can be viewed in real-time:

**[Go to the Data Visualization Site](https://korean-cuisine.cola172.store)**

### Precautions:

- **Service Interruptions due to Server Maintenance**: In the initial phase of the project, access to the service may occasionally be unavailable due to server maintenance.

- **Private Repository**: The code repository for the visualization site is not public.

## Future Plans

- We plan to continue working on the data until a meaningful dataset is built.
- The ultimate goal is to publish as an academic work through network and statistical analysis.

## Copyright Notice

### Ownership

- The owner of this project is Donghyeok, Choi from KAIST Graduate School of Culture Technology.
- The owner bears all legal responsibilities for the project and holds the rights.

### Terms of Use

- This project can only be used for **educational and academic purposes**.
- Commercial use is strictly prohibited.
- If you intend to use it for educational or academic purposes, you must attach the owner's name and repository link.

### Data Contribution

- Students taking the course are required to work on a minimum of 10 and a maximum of 13 data entries.
- If you wish to contribute more, please discuss with the owner.
- For inquiries about contributions, contact the owner's email ([dhchoi.lazy@gmail.com](mailto:dhchoi.lazy@gmail.com)).
- Contributions recognized will be differentially cited in academic papers.



---

# 한식의 기원

고려대학교 문과대학 디지털인문학입문II 05분반 프로젝트 데이터 업로드 저장소입니다.

## 개요

- 본 프로젝트는 고려대학교 문과대학 디지털인문학입문II 05분반 수업의 일환으로 진행됩니다.
- 디지털 인문학의 도구 사용법을 학습하고 해당 분야에 대한 이해를 심화시키는 것이 목적입니다.
- 근세부터 근대에 이르는 한국의 식재료와 조리법을 데이터로 수집하고, 이를 통해 '한식다움'이란 스타일이 무엇인지 탐구합니다.
- 이 프로젝트는 [이 연구](https://www.nature.com/articles/srep00196)로부터 영감을 받았으나, 우리의 연구 목표는 보편적인 food pairing 특성을 찾는 것이 아닌, 독특한 '한식의 특성'에 대한 탐구에 더 초점을 맞춥니다.
- 가을 학기 동안 우리가 수집할 조리서는 아래와 같습니다. 이 조리서들은 사료적 가치가 높고 이미 디지털화된 것도 있어 접근이 용이합니다.
  - 산가요록(山家要錄)
  - 음식디미방(閨壺是議方)
  - 수운잡방(需雲雜方)
- 향후 참고할 조리서의 목록은 한복려 선생님의 저서인 <[음식 고전](https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=94941877)>에서 발췌하였습니다. 저작권에 관한 문제가 발생할 경우, 아래 [저작권](#저작권) 섹션을 참조하여 주세요.

  ### 1400~1500년대 조리서

  - 산가요록(山家要錄) 식료찬요(食療纂要), 수운잡방(需雲雜方), 계미서(癸未書)

  ### 1600~1700년대 조리서

  - 도문대작(屠門大嚼), 최씨음식법(子孫寶傳), 신간구황촬요(新刊救荒撮要), 음식디미방(閨壺是議方), 요록(要錄), 주방문(酒方文), 음식보(飮食譜), 소문사설(謏聞事說), 증보산림경제(增補山林經濟)

  ### 1800년대 조리서

  - 규합총서(閨閤叢書), 임원경제지(林園經濟志), 동국세시기(東國歲時記), 윤씨음식법(饌法), 음식방문(飮食方文), 가기한중일월(可記閑中日月), 음식방문니라, 규곤요람(閨壼要覽), 주식시의(酒食是義), 이씨음식법(飮食法), 시의전서(是議全書)

  ### 1900년대 조리서

  - 반찬등속(饌膳繕冊), 부인필지(夫人必知), 조선무쌍신식요리제법(朝鮮無雙新式料理製法), 조선요리제법(朝鮮料理製法), 해동죽지(海東竹枝), 간편조선요리제법(簡便朝鮮料理製法), 사계의 조선요리(四季의 朝鮮料理), 조선요리법(朝鮮料理法), 가정주부필독(家庭主婦必讀), 조선요리학(朝鮮料理學), 우리음식, 이조궁정요리통고(李朝宮廷料理通考)

## 프로젝트 기여 방법

기여를 원하시는 모든 분들은 프로젝트 데이터에 기여할 수 있으며, 가을학기 종강 후에 기여를 시작해 주시면 감사하겠습니다.

이 프로젝트는 학생들의 Git/Github 사용 능력 향상을 목적으로 하기 때문에, 아래의 방법으로 기여해 주세요:

- Git 또는 Github에 익숙하지 않은 경우, [이 가이드](https://git-scm.com/book/ko/v2)를 참고하여 기본적인 사용법을 익히실 수 있습니다.
- Github에서 기여하실 때는 Pull Request를 통해 기여하실 수 있으며, [Pull Request 가이드](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)를 참조하세요.

### 데이터 기여 방법

1. `template.json` 파일을 다운로드하고, 각 필드에 대한 설명을 충분히 읽어주세요. 파일의 예시는 아래와 같습니다.

   ```json
   {
     "student_id": "학번, 이름, 닉네임 (일관되게 사용해 주세요)",
     "name": "음식 이름",
     "image": "images/your_image_name.png (이미지 파일은 images 폴더에 저장해 주세요. jpg 형식도 가능합니다.)",
     "image_prompt": "AI 이미지 생성에 사용한 프롬프트",
     "ingredients": ["식재료1", "식재료2", "식재료3"],
     "original": "원본 조리법을 여기에 입력합니다.",
     "translated": "조리법의 번역본을 여기에 입력합니다.",
     "source": "조리법의 출처를 여기에 입력합니다.",
     "comment": "이 음식에 대한 개인적인 생각이나 타인에게 알리고 싶은 정보를 여기에 입력합니다."
   }
   ```

#### 데이터 기여 방법 상세 안내

- **학번 (`student_id`)**: 문자열로만 구성해주세요. 파일 업로드 시 이를 파일명으로 활용합니다. 이미 존재하는 ID가 있을 경우 연번을 부여합니다.
- **음식명 (`name`)**: 개인 이름이 아닌 한식의 이름을 기입해야 합니다.
- **이미지 (`image`)**: 생성형 AI로 제작한 한식 이미지를 `images` 폴더에 업로드하고, 파일명은 `images/`로 시작해야 합니다.
- **프롬프트 (`image_prompt`)**: AI 생성 이미지에 사용한 프롬프트를 기재합니다. 완벽한 재현은 불가능하지만 유사한 결과를 얻는 데 도움이 됩니다.
- **식재료 (`ingredients`)**

  - **기본 규칙**: 목록은 리스트 형식으로 제출해야 하며, 수량이나 조리 상태는 포함하지 않습니다.

    | 입력 예시      | 설명                                       |
    | -------------- | ------------------------------------------ |
    | 불가: 콩 4~5되 | 수량은 기재하지 않습니다. '콩'으로 기재    |
    | 불가: 삶은 무  | 조리 상태를 기재하지 않습니다. '무'로 기재 |
    | 가능: 김치     | 김치찌개와 같은 조리법에서는 '김치'로 기재 |

- **원문 (`original`)**: 조리서의 원문을 여기에 기입합니다. 이는 데이터 수정 및 검증 시 사용됩니다.
- **번역 (`translated`)**: 한문이나 옛 한글인 경우, 번역문을 기재합니다. 이 프로젝트는 주로 식재료 사용을 확인하는 것을 목적으로 하므로 완벽한 번역은 필요하지 않습니다.
- **출처 (`source`)**: 출처가 되는 책 이름을 기재합니다. 한글로만 적되, 한자 병기는 허용하지 않습니다.
- **메모 (`comment`)**: 기타 참고할 만한 특이사항을 기재합니다.

#### 기여 절차

1. `template.json`을 `data` 폴더에 복사하고 원하는 이름으로 변경합니다.
2. `images` 폴더에 AI로 생성된 이미지를 업로드합니다. 파일명은 중복을 피해주세요.
3. Commit을 하고 자유롭게 메시지를 작성합니다.
4. Pull Request(PR)를 생성하고, 제목은 "학번 - 음식명"으로 합니다.
5. PR 승인을 기다립니다. 자동 스크립트로 형식을 검증합니다. 거절 시, 메시지를 확인하고 수정 후 재시도합니다.

## 데이터 시각화

결과물은 실시간으로 확인 가능합니다:

**[데이터 시각화 사이트 바로 가기](https://korean-cuisine.cola172.store)**

### 주의사항:

- **서버 유지 관리로 인한 중단**: 프로젝트 초기 단계인 현재에는 서버 유지 관리를 위해 종종 서비스 접근이 불가능할 수 있습니다.

- **저장소 비공개**: 시각화 사이트의 코드 저장소는 공개되지 않습니다.

## 향후 계획

- 의미 있는 데이터셋이 구축될 때까지 데이터 작업을 계속할 예정입니다.
- 최종 목표는 네트워크 및 통계 분석을 통해 학술 저작물로 출간하는 것입니다.

## 저작권 안내

### 소유권

- 본 프로젝트의 소유자는 KAIST 문화기술대학원 최동혁입니다.
- 소유자는 이 프로젝트에 대한 모든 법적 책임을 지며, 권리를 보유합니다.

### 사용 조건

- 본 프로젝트는 **교육 및 학술 목적**으로만 사용할 수 있습니다.
- 상업적 이용은 엄격히 금지되어 있습니다.
- 교육 및 학술 목적으로 활용하시려는 경우, 소유자와 저장소 링크를 반드시 첨부해야 합니다.

### 데이터 기여

- 수업의 수강생은 최소 10개, 최대 13개의 데이터 작업을 해야 합니다.
- 추가 기여를 원할 경우, 소유자에게 논의하세요.
- 기여도에 대한 문의는 소유자 이메일([dhchoi.lazy@gmail.com](mailto:dhchoi.lazy@gmail.com))로 연락 바랍니다.
- 기여도가 인정될 경우, 학술 논문에 차등 인용 예정입니다.

