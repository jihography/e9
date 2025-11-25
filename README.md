# e9

## main
1. `.Rmd` 코드 파일
- 아래 두 파일의 output은 업로드되어 있습니다.
    - (`SPM.Rmd`: sgis_sgg_merged 폴더 내의 SGG_MERGED.gpkg 이용, 공간가중행렬 구성 등)
    - (`data.Rmd`: 패널 데이터 이용해서 `dt_q_mod.csv`, `dt_y_mod.csv` 생성)'
- `model.Rmd`: 베이지안 계층 모형 적합

## `_data`
1. `.ipynb` 코드 파일
- `data_preprocessing.ipynb` : E9 비자 등록인원 패널 데이터로 전처리
- `matching_table.ipynb` : 시군구 단위 종속변수+설명변수 Join을 위한 Matching Table 구성
    - 각 데이터 소스별 unique 단위 추출
    - 행정구역 코드 베이스로 matching table 작성
    - table을 이용해 데이터 Join

2. `.csv` 파일
- `E9_panel_sgg_aggregated.csv`: 종속변수
- `population_panel_sgg_aggregated.csv`: 인구 (총/성별)
- `trade_panel.csv`: 수출입통계
- `unique_[src].csv`: `matching_table.ipynb`에서 생성된 unique (연도, 시군구) 쌍
- `matching_table_join_keys.csv`: matching table
- `panel_sgg_monthly.csv`: (test 용) Join된 데이터 파일

 