# Codyssey

코디세이 미션 저장소를 교육과정 순서대로 연결한 archive입니다. 프로젝트 코드와 Git 기록은 원본 저장소에 남고, 여기에는 서브모듈 참조만 저장합니다.

미션 제목과 순서는 **「코디세이 AI 올인원 학습 콘텐츠 소개」** PDF 3~7쪽을 기준으로 했습니다. PDF는 응용 과정의 첫 미션을 27번으로 표시하므로, 앞의 1~26번은 PDF에 실린 순서대로 부여했습니다. 기존 B 번호 및 과거 monorepo 번호와 다를 수 있습니다.

## 구조

```text
Codyssey/
├── basic/      # 입학연수(01~03), AI 도구학습(04~16)
├── advanced/   # AI 심화활용(17~26)
├── master/     # AI 응용·사업화(27~), 파이널 프로젝트
├── .gitmodules
└── README.md
```

확인된 저장소 23개를 연결했습니다. 미확인 미션에는 빈 서브모듈을 만들지 않았습니다.

## Clone

```bash
git clone --recurse-submodules https://github.com/shannonlee-dev/Codyssey.git
```

이미 clone했다면 `git submodule update --init --recursive`를 실행합니다.

## Basic — 입학연수

| 미션 | PDF의 미션 제목 | Repository | 상태 |
| --- | --- | --- | --- |
| 01 | 내 컴퓨터에 나만의 '작업실' 꾸미기 | [containerized-dev-workstation](https://github.com/shannonlee-dev/containerized-dev-workstation) | 확정 |
| 02 | 컴퓨터에게 명령 내리는 말(파이썬) 처음 배우기(퀴즈 게임) | [persistent-quiz-cli](https://github.com/shannonlee-dev/persistent-quiz-cli) | 확정 |
| 03 | AI가 계산하는 방식을 흉내 내는 작은 계산기 만들기 | [matrix-accelerator-simulator](https://github.com/shannonlee-dev/matrix-accelerator-simulator) | 확정 |

**7개 도메인 아이디어톤(텀 프로젝트)**은 제출 저장소를 확인하지 못해 연결하지 않았습니다.

## Basic — AI 도구학습

| 미션 | PDF의 미션 제목 | Repository | 상태 |
| --- | --- | --- | --- |
| 04 | 나만의 용돈 기입장 프로그램 만들기 | [personal-finance-cli](https://github.com/shannonlee-dev/personal-finance-cli) | 확정 |
| 05 | 나를 소개하는 웹페이지 처음부터 만들기 | [developer-portfolio-site](https://github.com/shannonlee-dev/developer-portfolio-site) | 확정 |
| 06 | 내가 고친 코드 설명을 AI가 대신 써주는 도우미 만들기 | [git-ai-assistant](https://github.com/shannonlee-dev/git-ai-assistant) | 확정 |
| 07 | 버튼 누르면 화면이 스르륵 바뀌는 요즘 웹사이트 만들기 (선택) | [study-notes-spa](https://github.com/shannonlee-dev/study-notes-spa) | 확정 |
| 08 | 친구 3~5명과 함께 프로그램 만드는 법 연습하기 (팀) | [git-flow-utility-lab](https://github.com/codyssey-b2-2-team-mission/git-flow-utility-lab) | 확정 |
| 09 | 내가 만든 웹사이트를 인터넷에 올려 누구나 쓰게 하기 | — | 불확실 |
| 10 | 컴퓨터가 알아서 자기 상태를 점검하게 만들기 | [linux-service-ops-automation](https://github.com/shannonlee-dev/linux-service-ops-automation) | 확정 |
| 11 | 파일이 언제 어떻게 바뀌었는지 기록하는 작은 프로그램 만들기 | [version-control-simulator](https://github.com/shannonlee-dev/version-control-simulator) | 확정 |
| 12 | 글을 쓰고·보고·고치고·지울 수 있는 게시판형 웹 서비스 만들기 (선택) | [book-records-crud-service](https://github.com/shannonlee-dev/book-records-crud-service) | 높은 확률 |
| 13 | 로그인이 되고 회원끼리 연결되는 웹 서비스 만들기 (선택) | [library-loan-management-service](https://github.com/shannonlee-dev/library-loan-management-service) | 높은 확률 |
| 14 | 정보를 엄청 빠르게 찾아주는 작은 저장소 만들기 | [mini-redis-data-structures](https://github.com/shannonlee-dev/mini-redis-data-structures) | 확정 |
| 15 | 컴퓨터가 갑자기 느려지거나 멈췄을 때 원인 찾아 고치기 | [system-failure-analysis-lab](https://github.com/shannonlee-dev/system-failure-analysis-lab) | 확정 |
| 16 | 정보를 깔끔하게 정리하는 디지털 서랍장 만들기 | [community-workshop-sql-lab](https://github.com/shannonlee-dev/community-workshop-sql-lab) | 확정 |

08은 팀 저장소 README에 PDF 미션 제목과 B2-2 과제 연결이 명시되어 있습니다. 09는 관련 후보 저장소가 있지만 PDF의 **여러 서비스 대시보드와 장애 대응 시연**을 확인하지 못했습니다. 12와 13은 주제는 맞지만 PDF의 API 및 외부 로그인 산출물과 구현 형태가 달라 확률을 구분했습니다.

## Advanced — AI 심화활용

| 미션 | PDF의 미션 제목 | Repository | 상태 |
| --- | --- | --- | --- |
| 17 | 쇼핑몰에서 누가 자주 오고 많이 사는지 분석해서 단골 찾기 | [customer-value-segmentation-pipeline](https://github.com/shannonlee-dev/customer-value-segmentation-pipeline) | 확정 |
| 18 | AI가 어떻게 학습하는지 수학으로 직접 풀어보기 | [model-learning-mechanics-lab](https://github.com/shannonlee-dev/model-learning-mechanics-lab) | 확정 |
| 19 | 휴대폰으로 찍은 종이를 똑바르게 펴서 스캔하게 만들기 | [document-digitization-pipeline](https://github.com/shannonlee-dev/document-digitization-pipeline) | 확정 |
| 20 | 영상 속 움직이는 사람·물건을 따라가며 표시해주기 | [motion-tracking-analysis-pipeline](https://github.com/shannonlee-dev/motion-tracking-analysis-pipeline) | 확정 |
| 21 | 원하는 내용이 들어있는 문서를 똑똑하게 찾아주는 검색기 만들기 | [document-retrieval-classification-system](https://github.com/shannonlee-dev/document-retrieval-classification-system) | 확정 |
| 22 | 글 속에 숨은 정보와 기분(좋음/나쁨)을 자동으로 뽑아내기 | [information-extraction-sentiment-engine](https://github.com/shannonlee-dev/information-extraction-sentiment-engine) | 확정 |
| 23 | 대출을 해줘도 될지 AI가 대신 판단해주는 시스템 만들기 | [customer-risk-explainability-pipeline](https://github.com/shannonlee-dev/customer-risk-explainability-pipeline) | 높은 확률 |
| 24 | AI가 어디서 자꾸 틀리는지 찾아내서 더 똑똑하게 만들기 | [predictive-model-diagnostics-pipeline](https://github.com/shannonlee-dev/predictive-model-diagnostics-pipeline) | 확정 |
| 25 | AI의 속 엔진(두뇌)을 내 손으로 직접 만들어보기 | — | 불확실 |
| 26 | CV, NLP 자율 주제 프로젝트 | — | repository 확인되지 않음 |

23은 위험 예측과 SHAP 설명을 함께 구현합니다. [credit-risk-modeling-pipeline](https://github.com/shannonlee-dev/credit-risk-modeling-pipeline)도 관련 작업이지만 PDF에 별도 신용 위험 미션이 없어 중복 연결하지 않았습니다. 25의 PDF 산출물은 이미지·글 결합 검색이므로, 직접 만든 신경망 엔진을 임의로 연결하지 않았습니다.

## Master — AI 응용·사업화 / 파이널 프로젝트

PDF의 응용 미션은 27번부터 시작합니다. 완료한 과정은 AI 심화활용까지이며, 확인된 응용·파이널 저장소는 아직 없습니다.

## 확인했으나 연결하지 않은 저장소

| Repository | 이유 |
| --- | --- |
| [secure-cloud-service-infra](https://github.com/shannonlee-dev/secure-cloud-service-infra), [fastapi-chatbot](https://github.com/shannonlee-dev/fastapi-chatbot) | 도구학습 09의 후보지만 PDF 산출물과 직접 일치하지 않음 |
| [credit-risk-modeling-pipeline](https://github.com/shannonlee-dev/credit-risk-modeling-pipeline) | 심화활용 23과 주제가 겹치나 별도 미션 근거가 없음 |
| [verified-neural-training-engine](https://github.com/shannonlee-dev/verified-neural-training-engine) | 심화활용 25의 멀티모달 검색 산출물과 다름 |
| [empty-repo](https://github.com/shannonlee-dev/empty-repo), [replay-curriculum-deep-rl-agent](https://github.com/shannonlee-dev/replay-curriculum-deep-rl-agent) | PDF의 완료 미션과 연결 근거가 부족함 |
| [langextract](https://github.com/shannonlee-dev/langextract), [tensorflow](https://github.com/shannonlee-dev/tensorflow), [free-llm](https://github.com/shannonlee-dev/free-llm) | 외부 프로젝트 포크 또는 별도 프로젝트 |
| [shannonlee-dev.github.io](https://github.com/shannonlee-dev/shannonlee-dev.github.io), [quant_modeling](https://github.com/shannonlee-dev/quant_modeling), [corpus](https://github.com/shannonlee-dev/corpus), [notion-easter-egg](https://github.com/shannonlee-dev/notion-easter-egg) | PDF 미션과 연결 근거가 없는 개인·연구 저장소 |

## 서브모듈 업데이트

기록된 커밋은 `git submodule status`로 확인합니다. 원본 저장소의 최신 커밋으로 올릴 때는 변경 내역을 검토하고 갱신된 gitlink를 커밋합니다.

```bash
git submodule update --remote --merge
git submodule status
git add basic advanced
git commit -m "chore: update Codyssey submodules"
```
