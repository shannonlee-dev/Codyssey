# Codyssey

코디세이 미션의 독립 Git 저장소를 submodule로 모은 archive입니다. 프로젝트 코드와 이력은 각 원본 저장소에 남습니다.

## 구조

```text
Codyssey/
├── admission/   # 입학연수: 개발환경, 퀴즈, AI 계산 체험
├── basic/       # AI 도구학습: B1-1 ~ B7-1
├── advanced/    # AI 심화활용: A1-1 ~ A6-2
├── master/      # AI 응용·사업화와 파이널 프로젝트
├── .gitmodules
└── README.md
```

현재 연결된 서브모듈은 27개입니다. 미션 코드는 디렉터리에서 바로 찾을 수 있으며, 원격 저장소 자체의 이름은 변경하지 않았습니다.

## Clone

```bash
git clone --recurse-submodules https://github.com/shannonlee-dev/Codyssey.git
```

이미 clone했다면 `git submodule update --init --recursive`를 실행합니다.

## Admission — 입학연수

| 경로 | 미션 제목 | Repository |
| --- | --- | --- |
| `admission/codyssey-01` | 내 컴퓨터에 나만의 '작업실' 꾸미기 | [containerized-dev-workstation](https://github.com/shannonlee-dev/containerized-dev-workstation) |
| `admission/codyssey-02` | 컴퓨터에게 명령 내리는 말(파이썬) 처음 배우기(퀴즈 게임) | [persistent-quiz-cli](https://github.com/shannonlee-dev/persistent-quiz-cli) |
| `admission/codyssey-03` | AI가 계산하는 방식을 흉내 내는 작은 계산기 만들기 | [matrix-accelerator-simulator](https://github.com/shannonlee-dev/matrix-accelerator-simulator) |

7개 도메인 아이디어톤의 제출 저장소는 확인되지 않아 연결하지 않았습니다. `01~03`은 이 archive에서 입학연수 항목을 구분하는 경로 번호이며 B 미션 번호가 아닙니다.

## Basic — AI 도구학습

아래 순서는 교육과정 표의 위에서 아래 순서입니다. B7-1 텀 프로젝트는 표 아래에 덧붙였습니다.

| 미션 | 미션 제목 | Repository | 상태 |
| --- | --- | --- | --- |
| B1-1 | 나를 소개하는 웹페이지 처음부터 만들기 | [developer-portfolio-site](https://github.com/shannonlee-dev/developer-portfolio-site) | 확정 |
| B1-2 | 버튼 누르면 화면이 스르륵 바뀌는 요즘 웹사이트 만들기 | [study-notes-spa](https://github.com/shannonlee-dev/study-notes-spa) | 확정 |
| B2-1 | 나만의 용돈 기입장 프로그램 만들기 | [personal-finance-cli](https://github.com/shannonlee-dev/personal-finance-cli) | 확정 |
| B2-2 | 친구 3~5명과 함께 프로그램 만드는 법 연습하기 | [git-flow-utility-lab](https://github.com/codyssey-b2-2-team-mission/git-flow-utility-lab) | 팀 저장소 확인 |
| B3-1 | 내가 만든 웹사이트를 인터넷에 올려 누구나 쓰게 하기 | [secure-cloud-service-infra](https://github.com/shannonlee-dev/secure-cloud-service-infra) | 높은 확률 |
| B3-2 | 내가 고친 코드 설명을 AI가 대신 써주는 도우미 만들기 | [git-ai-assistant](https://github.com/shannonlee-dev/git-ai-assistant) | 확정 |
| B4-1 | 컴퓨터가 알아서 자기 상태를 점검하게 만들기 | [linux-service-ops-automation](https://github.com/shannonlee-dev/linux-service-ops-automation) | 확정 |
| B4-2 | 컴퓨터가 갑자기 느려지거나 멈췄을 때 원인 찾아 고치기 | [system-failure-analysis-lab](https://github.com/shannonlee-dev/system-failure-analysis-lab) | 확정 |
| B5-1 | 정보를 엄청 빠르게 찾아주는 작은 저장소 만들기 | [mini-redis-data-structures](https://github.com/shannonlee-dev/mini-redis-data-structures) | 확정 |
| B5-2 | 파일이 언제 어떻게 바뀌었는지 기록하는 작은 프로그램 만들기 | [version-control-simulator](https://github.com/shannonlee-dev/version-control-simulator) | 확정 |
| B6-1 | 정보를 깔끔하게 정리하는 디지털 서랍장 만들기 | [community-workshop-sql-lab](https://github.com/shannonlee-dev/community-workshop-sql-lab) | 확정 |
| B6-2 | 글을 쓰고·보고·고치고·지울 수 있는 게시판형 웹 서비스 만들기 | [book-records-crud-service](https://github.com/shannonlee-dev/book-records-crud-service) | 높은 확률 |
| B6-3 | 로그인이 되고 회원끼리 연결되는 웹 서비스 만들기 | [library-loan-management-service](https://github.com/shannonlee-dev/library-loan-management-service) | 높은 확률 |
| B7-1 | 웹 기반 AI 챗봇 서비스 개발 텀 프로젝트 | [fastapi-chatbot](https://github.com/shannonlee-dev/fastapi-chatbot) | 제출 저장소의 개인 fork |

B2-2 팀 저장소에는 같은 미션 제목과 팀원 작업 이력이 있습니다. B3-1 저장소는 AWS 웹 서비스 인프라 구축을 구현하지만 PDF의 여러 서비스 대시보드 산출물은 확인되지 않았습니다. B6-2는 도서 CRUD 웹 앱, B6-3은 세션 인증 기반 도서 대여 서비스로, 각각 PDF의 게시판 API·외부 로그인 예시와 구현 형태가 다릅니다. B7-1은 `wilderif/codyssey-b7-1`에서 fork한 개인 저장소이며 README에 B7-1이 명시돼 있습니다.

## Advanced — AI 심화활용

표시 순서는 교육과정 표를 따릅니다. A5-2는 참고 번호표와 해당 저장소 구현에서 확인된 추가 미션으로, 오리엔테이션 PDF의 요약 표에는 별도 행이 없습니다.

| 미션 | 미션 제목 | Repository | 상태 |
| --- | --- | --- | --- |
| A1-1 | 쇼핑몰에서 누가 자주 오고 많이 사는지 분석해서 단골 찾기 | [customer-value-segmentation-pipeline](https://github.com/shannonlee-dev/customer-value-segmentation-pipeline) | 확정 |
| A2-1 | AI가 어떻게 학습하는지 수학으로 직접 풀어보기 | [model-learning-mechanics-lab](https://github.com/shannonlee-dev/model-learning-mechanics-lab) | 확정 |
| A3-1 | 휴대폰으로 찍은 종이를 똑바르게 펴서 스캔하게 만들기 | [document-digitization-pipeline](https://github.com/shannonlee-dev/document-digitization-pipeline) | 확정 |
| A3-2 | 영상 속 움직이는 사람·물건을 따라가며 표시해주기 | [motion-tracking-analysis-pipeline](https://github.com/shannonlee-dev/motion-tracking-analysis-pipeline) | 확정 |
| A4-1 | 원하는 내용이 들어있는 문서를 똑똑하게 찾아주는 검색기 만들기 | [document-retrieval-classification-system](https://github.com/shannonlee-dev/document-retrieval-classification-system) | 확정 |
| A4-2 | 글 속에 숨은 정보와 기분(좋음/나쁨)을 자동으로 뽑아내기 | [information-extraction-sentiment-engine](https://github.com/shannonlee-dev/information-extraction-sentiment-engine) | 확정 |
| A5-1 | 대출을 해줘도 될지 AI가 대신 판단해주는 시스템 만들기 | [credit-risk-modeling-pipeline](https://github.com/shannonlee-dev/credit-risk-modeling-pipeline) | 확정 |
| A5-2 | 고객 위험 군집화와 판단 근거 설명 | [customer-risk-explainability-pipeline](https://github.com/shannonlee-dev/customer-risk-explainability-pipeline) | PDF 요약 외 추가 확인 |
| A6-2 | AI가 어디서 자꾸 틀리는지 찾아내서 더 똑똑하게 만들기 | [predictive-model-diagnostics-pipeline](https://github.com/shannonlee-dev/predictive-model-diagnostics-pipeline) | 확정 |
| A6-1 | AI의 속 엔진(두뇌)을 내 손으로 직접 만들어보기 | [verified-neural-training-engine](https://github.com/shannonlee-dev/verified-neural-training-engine) | 높은 확률 |
| — | CV, NLP 자율 주제 프로젝트 | — | 제출 저장소 확인되지 않음 |

A6-1은 직접 만든 학습 엔진이라는 제목과 부합하지만, PDF에 적힌 이미지·글 결합 검색 산출물과는 차이가 있습니다.

## Master — AI 응용·사업화 / 파이널 프로젝트

현재 완료한 과정은 AI 심화활용까지입니다. 확인된 응용·파이널 저장소는 아직 없습니다.

## 서브모듈 업데이트

```bash
git submodule status
git submodule update --remote --merge
git add admission basic advanced
git commit -m "chore: update Codyssey submodules"
```

각 프로젝트의 브랜치·이슈·PR과 코드 이력은 원본 저장소에서 관리합니다.
