# 202112707_node_final

## Table
### Countries
|columns|description|
|---|---|
|id|기본키|
|alpha2Code|ISO 3166-1 alpha-2 code|   
|alpha3Code|ISO 3166-1 alpha-3 code|   
|numericCode|ISO 3166-1 numeric code|   
|nameKR|한글 국가명|
|nameEN|ISO 3166-1 영문 국가명|
|createdAt|작성일시|
|updatedAt|수정일시|

데이터 예시

![country data](https://user-images.githubusercontent.com/73145656/122716676-85bb1800-d2a5-11eb-8cba-633afaea38aa.PNG)


### Subdivisions 
|columns|description|
|---|---|
|id|기본키|
|code|ISO 3166-2 code|   
|nameKR|한글 행정구역명|
|nameEN|영문 행정구역명|
|createdAt|작성일시|
|updatedAt|수정일시|

데이터 예시

![subdivisiondata](https://user-images.githubusercontent.com/73145656/122716683-881d7200-d2a5-11eb-8356-30c742912f29.PNG)

---
## base url: http://3.37.62.54:3000
## 메소드
|method|url|
|---|---|
|Get | /country|
| Get | /country/:alpha2_code|
| Post | /country|
| Put | /country|
| Delete | /country|
| Get | /subdivision|
| Post | /subdivision|
| Put | /subdivision           |
| Delete | /subdivision|
#
### Get /country 
#### 업무 - 국가 목록 보기
#### 응답 - JSON
- msg - 성공/실패 메시지
- data
- 예시

![image](https://user-images.githubusercontent.com/73145656/122719576-53131e80-d2a9-11eb-8053-4b5a527db03e.png)
#
### Get /country/:alpha2_code
#### 업무 - alpha2_code 에 해당하는 국가의 정보와 행정구역 보기
#### 응답 - JSON
- msg - 성공/실패 메시지
- data
- 예시

![image](https://user-images.githubusercontent.com/73145656/122720452-738fa880-d2aa-11eb-8f23-7adce3fc93d2.png)
#

### Post /country
#### 업무 - 국가 정보 등록
#### 요청 바디

![image](https://user-images.githubusercontent.com/73145656/122723216-a7200200-d2ad-11eb-9376-5a6da9605c3d.png)


#### 응답 - JSON
- msg - 성공/실패 메시지
#

### Put /country
#### 업무 - 전달 받은 id에 해당하는 국가 정보 수정
#### 요청 바디

![image](https://user-images.githubusercontent.com/73145656/122723286-c1f27680-d2ad-11eb-99ab-111f4f63a450.png)


#### 응답 - JSON
- msg - 성공/실패 메시지
#

### Delete /country
#### 업무 - 전달 받은 id에 해당하는 국가 정보 삭제
#### 요청 바디
- id - 삭제할 Country 레코드 id
#### 응답 - JSON
- msg - 성공/실패 메시지
#

### Get /subdivision
#### 업무 - 등록된 행정구역 보기
#### 응답 - JSON
- msg - 성공/실패 메시지
- data
- 데이터 예시

![image](https://user-images.githubusercontent.com/73145656/122722658-f0238680-d2ac-11eb-8bc9-e21b7e685ce9.png)
#

### Post /subdivision
#### 업무 - 행정구역 등록
#### 요청 바디

![image](https://user-images.githubusercontent.com/73145656/122723014-67591a80-d2ad-11eb-88c7-05bc13956c37.png)
#### 응답 - JSON
- msg - 성공/실패 메시지
#
### Put /subdivision
#### 업무 - 행정구역 정보 수정
#### 요청 바디

![image](https://user-images.githubusercontent.com/73145656/122723894-68d71280-d2ae-11eb-9558-78a5ec42ce07.png)
#### 응답 - JSON
- msg - 성공/실패 메시지
#

### Delete /subdivision
#### 업무 - 전달 받은 id에 해당하는 행정구역 정보 삭제
#### 요청 바디
- id - 삭제할 subdivision 레코드 id
#### 응답 - JSON
- msg - 성공/실패 메시지
#
