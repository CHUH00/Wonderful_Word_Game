<div align="center">

# 🎮 원더풀 워드 게임 (Wonderful Word Game)
### 🧩 자연어 처리(NLP) 단어 유사도 기반의 인터랙티브 콘솔 게임

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

</div>

## 📌 프로젝트 소개
**원더풀 워드 게임 (Wonderful Word Game)** 은 실제 대화형 자연어 처리(NLP) 데이터셋을 활용해 구축된 창의적인 콘솔 텍스트 게임입니다. 

단순히 하드코딩된 정답을 맞히는 것이 아니라, "한국어 단발성 대화 데이터셋"에 내재된 **질문(Q) - 응답(A)** 의 컨텍스트(1:1 매칭 구조)를 직접 게임 로직으로 승화시켰습니다. 사용자는 AI가 제시하는 문장을 보고 올바른 응답을 추론하거나 단어 유사도를 분석하며 언어적 감각을 키울 수 있습니다.

## 📊 데이터셋 및 대응 기준 로직
- **활용 데이터**: `한국어_단발성_대화_데이터셋.xlsx`
- **게임 알고리즘**:
  1. 엑셀 형태의 대화형 데이터셋을 `Pandas`를 이용해 데이터프레임으로 로드합니다.
  2. 컬럼 간의 유의미한 질의-응답 짝을 난수로 추출하여 게임의 **제시어(문제)**로 화면에 띄웁니다.
  3. 사용자는 문맥적으로 올바른 쌍을 이루는 정답 해시나 문장을 입력해야 인정 처리되며 스코어가 누적됩니다.

## 📺 게임 실행 및 전처리 화면

현업 데이터 분석 환경답게 데이터 전처리부터 철저히 수행한 뒤 본 게임 로직 진입을 시도합니다. 결측치 및 중복값을 정리하는 과정이 콘솔에 모두 시각화됩니다.

### 🔹 데이터 정제 단계 (Preprocessing)
<div align="center">
  <img src="images/전처리전.png" alt="전처리 전 원본 데이터" width="45%" style="margin:5px;" />
  <img src="images/전처리후.png" alt="전처리 완료된 데이터" width="45%" style="margin:5px;" />
</div>

### 🔹 단어 유사도 판별 및 메인 게임 루프
단어들의 의미론적인 유사도를 판별한 뒤, 텍스트 게임 프롬프트를 띄워 사용자와 상호작용합니다.
<div align="center">
  <br>
  <img src="images/단어유사도.png" alt="단어 유사도 검증 로직" width="70%" style="margin-bottom:10px;" />
  <br>
  <img src="images/게임화면.png" alt="실제 게임 플레이 콘솔" width="70%" />
</div>

---
*본 프로젝트는 자연어 처리 데이터의 정제 및 활용 방안, 알고리즘 구현 기법에 대한 탐구의 일환으로 [우진(Woojin Choi)](https://github.com/CHUH00)에 의해 개발되었습니다.*
