# data/

원본 CSV를 두는 폴더입니다. 저장소에는 포함하지 않았으므로(`.gitignore`로 제외) 직접 내려받아 아래 파일명으로 넣어 주세요.

출처: 서울 열린데이터광장 서울시 상권분석서비스 (2025년 1~4분기, 25개 자치구, 1,650개 상권)

| 파일명 | 내용 | 인코딩 | 링크 |
|---|---|---|---|
| `seoul_commercial_district_master_2025.csv` | 상권 위치 정보(자치구, 행정동, 좌표) | cp949 | 서울 열린데이터광장 상권분석서비스 |
| `seoul_commercial_district_stores_2025.csv` | 상권×업종×분기 점포 수, 개업·폐업 | cp949 | https://data.seoul.go.kr/dataList/OA-15577/S/1/datasetView.do |
| `seoul_commercial_district_attraction_facilities_2025.csv` | 상권 주변 집객시설 수(연 1회 갱신) | utf-8-sig | https://data.seoul.go.kr/dataList/OA-15580/S/1/datasetView.do |

파일마다 인코딩이 다르니 직접 읽을 때는 위 표대로 `encoding`을 지정하세요. 컬럼 구조는 [`notebooks/01_데이터_탐색.ipynb`](../notebooks/01_데이터_탐색.ipynb), 원본 데이터의 오류와 보정은 [`notebooks/02_EDA_상권쇠퇴분석.ipynb`](../notebooks/02_EDA_상권쇠퇴분석.ipynb)에서 볼 수 있습니다.

노트북이 만드는 정제 CSV는 `data_clean/`에 저장됩니다(`notebooks/06` 실행 결과).
