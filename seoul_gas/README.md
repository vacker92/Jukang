## 분석 주제
서울시 도시가스 이용 가구수, 인구, 소득 데이터를 활용한 **에너지 소비 특성 분석 및 클러스터링**

##  분석 목적
서울시 자치구별 에너지 소비 특성과 지역간의 패턴을 파악해보며, 지역별 에너지 취약성 및 효율성을 평가 할수 있다.

### 데이터 출처

1. 서울시 도시가스 이용 현황 (2019~2023)
  [서울열린데이터광장](https://data.seoul.go.kr/dataList/125/S/2/datasetView.do)
    - 서울시 자치구별 도시가스 공급량 및 사용량 (연도별)
    - [데이터 전처리 후 mysql 업로드](https://github.com/vacker92/Jukang/blob/main/seoul_gas/gas_sql.ipynb)

---

2. 서울시 상주인구
[서울열린데이터광장](https://data.seoul.go.kr/dataList/OA-22182/S/1/datasetView.do)
    - 서울시 자치구별 상주인구 (총인구, 성별, 연령별)
    - [데이터 전처리 후 mysql 업로드](https://github.com/vacker92/Jukang/blob/main/seoul_gas/population_sql.ipynb)

---

3. 서울시 소득소비 통계
[서울열린데이터광장](http://data.seoul.go.kr/dataList/OA-22167/S/1/datasetView.do)
    - 가구당 월 평균 소득 및 지출 항목 (자치구기준, 연도별제공)
    - [데이터 전처리 후 mysql 업로드](https://github.com/vacker92/Jukang/blob/main/seoul_gas/income_sql.ipynb)

---

4. 서울시 지도 GeoJSON
[GeoJSON 지도 파일](https://raw.githubusercontent.com/southkorea/seoul-maps/master/kostat/2013/json/seoul_municipalities_geo_simple.json)


## 활용 기술 
ubuntu (mysql)  
python (pandas, matplotlib, seaborn, sklearn, geopandas)  
KMeans 클러스터링
