# 공공기관 데이터 분석 프로젝트

## 프로젝트 개요
안전정보 데이터를 활용하여 공공 안전과 관련된 동향을 분석하고, 데이터 기반의 유용한 인사이트를 제공하는 프로젝트입니다. 데이터 수집부터 정제, 분석 및 시각화를 통해 공공 안전 데이터의 활용 가능성을 탐구합니다.

## 프로젝트 배경
블랙아이스(결빙 도로) 사고는 겨울철 교통사고의 주요 원인 중 하나로, 도로의 결빙 여부를 육안으로 확인하기 어렵기 때문에 운전자들에게 큰 위험을 초래합니다. 이에 따라, 블랙아이스와 관련된 데이터 기반 분석 및 예측이 공공 안전 향상에 필수적이라고 판단했습니다.
본 프로젝트는 블랙아이스 사고와 같은 위험 요소를 데이터로 분석하여, 예방 조치를 지원하고 관련 기관과 협력하여 실질적인 공공 안전 개선을 목표로 하고 있습니다. 이를 통해 블랙아이스 사고를 사전에 방지하고, 관련 데이터의 활용성을 높이고자 합니다.

## 주요 목표
- 안전정보 포털 API와 웹 크롤링(동적, 정적)을 활용하여 데이터를 수집합니다.
- 수집된 데이터를 정제하여 분석 가능한 형태로 가공합니다.
- 데이터 시각화를 통해 주요 트렌드 및 통계 정보를 파악합니다.
- 공공 안전 데이터의 활용 사례를 제시합니다.

## 사용 기술
- **언어**: Python
- **라이브러리**: 
  - 데이터 수집: `requests`, `selenium`, `beautifulsoup4`
  - 데이터 분석: `pandas`, `numpy`
  - 데이터 시각화: `matplotlib`, `seaborn`, `plotly`,`WordCloud`
- **데이터 저장**: `JSON`, `CSV`, `Pickle`
- **배포 및 협업**: Visual Studio Code, Jupyter Notebook

## 주요 기능
1. **데이터 수집**
   - 안전정보 포털 API를 활용하여 데이터를 자동으로 수집합니다.
   - Selenium과 BeautifulSoup을 활용한 동적/정적 웹 크롤링으로 추가 데이터 확보.

2. **데이터 정제 및 분석**
   - 중복 데이터 제거, 결측치 처리, 데이터 정규화 등 데이터 정제 작업 수행
   - 공공 안전과 관련된 주요 지표를 분석

3. **데이터 시각화**
   - 안전 정보 통계 데이터 시각화
   - 특정 지역 또는 기간에 대한 트렌드 분석
   - 위험 요소와 관련된 히트맵 생성

## 설치 및 실행 방법
1. 프로젝트 클론
   ```bash
   git clone https://github.com/jjw9728/Project
   cd Project
   ```

2. 가상환경 생성 및 활성화
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows의 경우 venv\Scripts\activate
   ```

## 프로젝트 구조
```
notebooks/
├── 00.crawling_data.ipynb
├── 01.api_data_collection.ipynb
├── 02.map_visual.ipynb
├── 03.temp_visual.ipynb
├── 04.rainfall_visual.ipynb
├── 05.Temperature_Rainfall_Risk_Trend.ipynb
├── 06.Rainfall_Risk_Distribution_Visualization.ipynb
├── 07.Rainfall_Risk_Relationship.ipynb
├── 08.Temperature_Risk_Relationship.ipynb
├── 09.Temperature_Risk_Factor_Analysis.ipynb
├── 10.Midterm_Weather_Coordinate_Based_Analysis.ipynb
└── 11.Weather_Crawling_Risk_Analysis_Automation.ipynb
```

## 결과 예시
- 지역별 안전 데이터 시각화 그래프
- 시간별 안전 사건 발생 추이
- 위험 요소 히트맵

## 향후 계획
- 추가적인 공공 데이터 포털 API 통합
- 대규모 데이터 분석을 위해 클라우드 기반 데이터 처리 플랫폼 도입
- 실시간 알림 및 위치 기반 서비스를 통해 정부와 협력하는 방안을 모색

## 기여 방법
프로젝트에 기여하고 싶다면, 다음 절차를 따라주세요:
1. 원격 저장소에서 새로운 브랜치를 생성합니다. (`git branch feature-branch`)
2. 생성한 브랜치로 이동합니다. (`git checkout feature-branch`)
3. 작업을 완료한 후, 해당 브랜치에 커밋과 푸시를 수행합니다.
4. 팀원들과 협의 후 `main` 브랜치에 병합합니다.

## 역할 분담
- [황세진](https://github.com/sejin1048) : 데이터 분석 및 정제, 데이터 시각화, 발표, 데이터 조사
- [조재원](https://github.com/jjw9728): 데이터 분석 및 정제, 데이터 시각화, API 활용을 통한 데이터 저장 및 크롤링
- [이경준](https://github.com/KYEONGJUN-LEE): 데이터 분석 및 정제, 데이터 시각화, API 활용을 통한 데이터 저장 및 크롤링
- [류경미](https://github.com/ggmmi1) : 데이터 분석 및 정제, 데이터 시각화, 데이터 조사, 발표 자료 제작
