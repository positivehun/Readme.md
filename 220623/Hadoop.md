
# 빅데이터

## 빅데이터 저장
### 데이터 소스 -> 수집 -> 저장 -> 처리 -> 분석 -> 표현
### 데이터소스 -> 내부데이터 외부데이터 미디어
### 수집 -> 수동 자동(로그수집기 크롤링 센싱)
### 저장 -> 정형,비정형,데이터등급 / 저장장치
### 처리 -> 일괄처리 실시간&배치 분산병렬처리
### 분석 -> 전처리, 분석방법론
### 표현 -> 시각화

## <하둡(HADOOP)>

### 대용량 데이터를 분산 처리할 수 있는 자바기반의 오픈소스 프레임워크
### DBMS가 아닌 프레임워크
### 하둡은 분산시스템인 HDFS에 데이터를 저장하고 맵리듀스를 이용해 데이터를 처리
### HDFS(Hadoop Distributed File System)
### -> 빅데이터 파일을 여러대의 서버에 분산 저장하기 위한 파일시스템
### Map Reduce(분산처리)
### -> 각 서버에서 데이터를 분산처리하는 분산 병렬처리를 위한 분석 시스템
## The Apache Hadoop Stack
### <Hadoop User Experience (HUE)>
|역할|툴|
|:--:|:--:|
|Data Exchange|Sqoop| 
|Log Control|Flume|
|Coordination|Zoo keeper|
|Scripting|Pig|
|SQL|Hive|
|ML|Mahout|
|Worlkflow|Oozie|
|Columnal data store|HBase|
|etc|YARN/Map Reduce/HDFS(Hadoop Distributed File System)|


## <하둡의 역사>
### DBMS의 한계
### -> 웹 크롤러 색인처리 과정에서 매우 큰 파일 처리의 한계
### 하둡 -> 텍스트 검색 라이브러리로 폭넓게 사용되고 있는 아파치 루쓴의 창시자인 더그커팅에 의해 시작
### 크롤러와 함께 검색엔진 시스템 성능 향상

## <검색엔진의 작동 원리>
### 스파이더,크롤러라고 불리는 로봇이 웹에 있는 웹페이지를 방문해서 모든 내용을 읽어옴
### 검색에 적합하도록 일정하게 가공하여 저장





