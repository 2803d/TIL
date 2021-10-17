# Flight

- 2019~2020년 항공 데이터를 태블로를 사용하여 시각화/분석

## 항목
### 기본 정보
- Record Id : Id
- Scheduled Date : 날짜
- Regular or Irregular : 정기/부정기
- Domestic or International : 국내선/국제선
- Departure or Arrival : 출발/도착 구분

### 항공사
- Airline Icao, Nm : 항공사 코드/이름
- Airline Category : 항공사 코드 정보
	- 0 : 외항수
	- 1 : 대한항공
	- 2 : 아시아나항공 ...

### 탑승지/도착지 정보
- Airport Nm, Cd, Lat, Long : 공항 이름/코드/위도/경도
- Corresponding Cd, Lat, Long : 도착지/출발지 공항 코드/위도/경도
- Continent Group, Subgroup, Country, City : 해당 대륙, 국가, 도시

### 정상운행/지연/결항
- Flight Plan : 계획 된 항공편? 전부 1
- Flight Happened : 실제로 운행했는지 여부
- Flight Delayed, Delay Cd : 항공편 지연 여부, 지연 코드
	- <delay cd>  [0 : 지연 없음, 1 : 기상지연, 3 : 정비지연, 4 : 항로혼잡, 5 : 여객처리, 6 : 기타지연]
- Flight Canceled, Cancel Cd : 항공편 취소 여부, 취소 코드
	- <cancel cd> [0 : 결항 없음, 1 : 기상 결항, 2 : 접속 결항, 3 : 정비결항, 4 : 기타걸형]

### 승객
- Passengers Charged, Transfer : 탑승 승객수, 환승 승객 수

### 수하물
- Baggage/Freight/Mail Kg : 수하물/화물/우편 무게


## 살펴 볼 부분
1. 날짜별(월별, 년도별 등) 데이터 분석
2. 출발/도착 지역별 비교, 지도와 어떻게 연관 지을지
3. 항공사별 데이터 분석
4. 결항/지연된 항공편들의 특징 분석(각 코드별 : 항공사의 문제? 기상 문제?)
5. 정기/부정기, 국제선/국내선 분석

