| no |데이터명|컬럼명|설명|예시|
|:--:|:----------|:----------|:------------|:------------|
|1|Case.csv	        |case_id	                |감염케이스 id	                            |1000001, 1000002, ...       |
| |                 |province                 |특별시/광역시/도                         |Seoul, Busan, ...           |
|	|               	|city                     |구/시                                  |Yongsan-gu, Guro-gu, ...    |
|	|	                |group                    |집단감염 유/무                          |True, False                 |
|	|	                |infection_case           |감염 케이스(그룹명)                     |Itaewon Clubs, ...          |
|	|               	|confirmed                |확인 된 누적 수                          |133.0, 99.0, ...            |
|	|	                |latitude                 |위도                                    |37.538621, ...              |
|	|	                |longitude                |경도                 	                 |126.992652, ...              |
|2|PatientInfo.csv  |patient_id	              |감염케이스 id	                          |1000000001, 1000000002, ...|
|	|	                |global_num               |질병관리청으로부터 부여받은 번호	        |2.0, 5.0, ...              |
|	|               	|sex                      |성별      	                            |male, female, ...|
|	|	                |birth_year               |출생년도	                               |1964, 1987, ...         |
|	|	                |age	                    |나이                           	      |50s, 30s, ...               |
|	|               	|country              	  |국가	                                    |Korea|
|	|	                |province	                |특별시/광역시/도                          |Seoul|
|	|               	|city           	        |구/시	|Gangse-gu|
|	|               	|disease                  |기저질환 여부|	NaN|
|	|               	|infection_case	          |감염 케이스|	overseas inflow|
|	|               	|infection_order	        |감염 순서|	1.0, 1.0, ...|
|	|	                |infected_by	            |감염시킨 사람 id|	NaN, 20020000001|
|	|               	|contact_number           |사람들과 접촉 수|	75|
|	|               	|sympton_onset_date       |증상 발병 날짜	|2020-01-22, NaN|
|	|               	|confirmed_date	          |확진 일자	|2020-01-23, 2020-01-30, ...|
|	|               	|realeased_date	          |발병 일자	|2020-02-05, 2020-03-02, ...|
|	|               	|deceased_date	          |사망 일자	|NaN|
|	|               	|state                    |상태	|isolated / released / deceased|
|3|PatientRoute.csv |patient_id               |환자 id|1000000001|
|	|               	|global_num               |질병관리청으로부터 부여받은 번호|	2.0, 5.0, ...|
|	|	                |date                     |년월일	|2020-01-22, 2020-01-24, ...|
|	|               	|province	                |특별시/광역시/도	|Gyeonggi-do, Seoul, ...|
|	|	                |city	                    |구/시|	Gimpo-si, ...|
|	|	                |type	                    |장소	|airport, hospital, etc, ...|
|	|	                |latitude	                |위도	|37.615246, 37.567241, ...|
|	|	                |longitude	              |경도	|126.715632, 127.005659, ...|
|4|Time.csv         |date                     |년월일||
|	|	                |time	                    |시간||
|	|	                |test	                    |코로나 테스트 누적 합||
|	|               	|negative	                |누적 음성 수||
|	|	                |confirmed                |누적 확진자 수||
|	|               	|released                 |누적 발병 수||	
|	|	                |deceased                 |누적 사망자 수|	|
|5|TimeAge.csv      |date                     |년월일||
|	|	                |time                     |시간|	|
|	|	                |age                      |환자 나이||	
|	|               	|confirmed                |누적 확진자 수||
|	|	                |deceassed                |누적 사망자 수|	|
|6|SeoulFloating.csv|date                     |년월일         ||
|	|	                |hour                     |시간|	|
|	|               	|birth_year               |출생년도||
|	|               	|sex                      |성별|	|
|	|	                |province                 |특별시/광역시/도||
|	|               	|city                     |구/시||	
|	|	                |fp_num                   |유동인구 수||
|7|SearchTrend.csv  |date                     |년월일| |	
|	|	                |cold                     |한국어 '감기' 검색량|	|
|	|               	|flu                      |한국어 '독감' 검색량|	|
|	|               	|pneumonia                |한국어 '폐렴' 검색량||
|	|	                |coronavirus              |한국어 '코로나 바이러스' 검색량|	|
|8|Weather.csv      |code                     |지역코드      | |
|	|                	|province                 |특별시/광역시/도	|Gyeonggi-do, Seoul, ...|
|	|               	|date                     |년월일 | |		
|	|	                |avg_temp                 |평균기온	| |		
|	|               	|min_temp                 |최저기온	| |		
|	|               	|max_temp                 |최고기온	| |		
|	|               	|precipitation            |강수량	| |		
|	|	                |max_wind_speed           |최대풍속	| |		
|	|               	|most_wind_direction      |풍향(most frequent)	| |		
|	|	                |avg_relative_humidity    |평균습도| |		
|9|TimeGender.csv   |date                     |년월일	| |		
|	|               	|time                     |시간	| |		
|	|	                |sex                      |성별	| |		
|	|               	|confirmed                |누적 확진자 수	| |		
|	|               	|deceased                 |누적 사망자 수	| |		
|10|TimeProvince.csv|date                     |년월일	| |				
|	|                	|time                     |시간| |		
|	|	                |province                 |특별시/광역시/도	|Gyeonggi-do, Seoul, ...|
|	|	                |confirmed                |지역 내 누적 확진자 수	| |		
|	|               	|released                 |지역 내 누적 발병 수	| |		
|	|	                |deceased                 |지역 내 누적 사망자 수	| |	
|11|Policy.csv      |policy_id                |정책id| |				
|	|               	|country                  |정책 시행 국가명| |		
|	|               	|type                     |정책 종류	| |		
|	|	                |gov_policy               |정부 정책| |		
|	|               	|detail                   |정책 설명| |		
|	|	                |start_date               |정책 시작일	| |		
|	|	                |end_date                 |정책 종료일| |	
|12|Region.csv      |code                     |지역 코드| |				
|	|	                |province                 |특별시/광역시/도	|Gyeonggi-do, Seoul, ...|
|	|               	|city                     |구/시/군||	
|	|                	|latitude                 |위도| |		
|	|               	|longitude                |경도| |		
|	|	                |elementary_school_count  |초등학교 수| |		
|	|	                |kindergarten_count       |유치원 수| |		
|	|               	|university_count         |대학교 수| |		
|	|                	|academy_ratio            |전문대 비율| |		
|	|               	|elderly_population_ratio |노인 인구 비율| |		
|	|	                |elderly_alone_ratio      |독거 노인 비율| |		
|	|	                |nursing_home_count       |요양원 수| |		
