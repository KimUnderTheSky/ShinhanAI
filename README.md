# SAR : 리츠투자플랫폼 

<p align='center'>
<br>
<div align="center">
 <img width="80%" src="https://github.com/ssongssong00/ShinhanAI/assets/87919319/e6783a9a-8838-4732-ab3c-55de0e803af8"/>

</div>

</p>

SAR은 리츠 투자자의 리츠 가치평가를 돕는 대시보드로 
* 한 달뒤 상장 리츠 주가 등락 예측, 
* 대안 정보를 활용한 대시보드,
* 리츠 활성화를 이루고자 합니다.

## 🗂️프로젝트 소개
본 프로젝트는 상장리츠 대시보드와 주가예측 등락 모델을 통해,  
* 리츠 회사와 일반 투자자간 **정보비대칭을 해소**하고,
* 리츠 회사의 **배당수익률 단편 정보의 문제를 해결**하고.
* 리츠의 전반적인 특성(회계, 부동산 정보)를 고려한 주가등락예측 모형으로 **예측 정보**를 제공해
* 궁극적으로 투자자들이 **신중하고 현명한 투자를**하는 것에 목표를 둡니다.


## 📠관련 문서
<details>
 <summary>📃주제 정의 문서</summary>
 
 ### 아이디어 제안 배경
   - 2023년 3월말 기준 리츠의 총자산**연평균 성장률은 28.6%** 로 리츠시장이 빠르게 성장하고 있습니다. 
   - 정부의 **공모•상장 리츠 활성화 정책**으로 리츠시장이 더욱 확장될 것으로 기대됩니다.
   - 고령인구 증가로 **인컴형 자산(리츠)**을 통한 은퇴설계 니즈가 증가하고 있습니다. 
   - 22년 말 저점을 찍은 리츠 주가가 23년 금리인상 사이클 종료와 함께 회복세에 진입하기 전 23년 1분기가 리츠 투자 적기입니다. 
   
 
 ### 사례분석을 통한 문제 발견
 **에이리츠 배당수익률 단편 정보 문제**
 - 다른 리츠의 비해 매우 높은 배당수익률로 **투자자들의 거래**가 이루어지고 있습니다.
 - **에이리츠의 회계공시자료**를 통해 거래정지 이력이 있어 재정상태가 적절하지 않음을 확인했습니다.
 - **에이리츠의 기초자산**을 조사했을 때 부동산 시장이 가장 침체된 지역의 사업 진행예정중입니다.
 -> 에이리츠는 투자자들에게 높고 안정적인 배당을 지급할 가능성이 매우 낮지만 여전히 투자자들의 거래가 이루어짐을 확인할 수 있습니다. 

 ### 사례분석을 통한 문제 정의
 - 일반투자자들이 안전한 리츠 투자를 하기 위한
1. 리츠 중심의 회계 정보 부족 및 부재
(미국과 달리 한국은 일반 상장기업과 다른 리츠 가치평가 계정과목이 제공안됨- FFO,NOI,Cap rate)
2. 리츠회사가 보유한 부동산 정보 부족
(리츠정보시스템은 현재 정보의 부족 및 부재로 인해 정보비대칭 해소 역할을 달성하지 못한 상황) 

 
 ### 아이디어 내기 
 - FFO,NOI등 리츠 가치평가 회계정보들을 계산해 대시보드로 제공
 - 리츠회사가 보유한 부동산의 지리적,경제적(상권)에 대한 정보를 대시보드 제공 
 - 머신러닝 및 딥러닝 모델에 기반한 상장 리츠 주가 등락 예측 정보 제공
 - 거시적인 시장 상황을 반영한 부동산 섹터별 시장 심리 정보 제공
 
</details>

<details>
 <summary>🗒사용자 정의 문서</summary>
 
 ### 페르소나
 ![P_LOW 페르소나-001](https://user-images.githubusercontent.com/87919319/225295722-e8ef7b51-4cee-414b-8276-a617d9a27f48.png)

 ### 시나리오
 
 #### #1
 *대한적십자사 직원인 나대한은 헌혈의 집에서 헌혈자의 헌혈을 도운다.*
 
 0. 나대한은 웹 페이지를 실행한다.
  0-1. 본인의 개인키로 로그인하여 대한적십자사 전용 페이지에 접근한다.
 1. 나대한은 헌혈자가 헌혈을 마치고 나오면 헌혈자의 정보를 양식에 입력한다.
 2. 입력을 한 후, 발행 버튼을 눌러 해당 헌혈자에게 NFT 헌혈증명서를 발행한다.
 3. 발행 기록을 통해 지금까지 자신이 발행한 NFT 헌혈증명서를 확인한다. 
 
 #### #2
 *헌혈을 처음 하는 대학생 홍길동은 헌혈을 마치고 나온다.*

 0. 홍길동은 처음으로 웹 페이지를 실행한다. 
  0-1. 본인의 개인키로 로그인하여 헌혈자 전용 페이지에 접근한다.
 1. 방금 헌혈한 기록을 NFT 헌혈증명서를 통해 확인한다.
 2. 헌혈증서 커뮤니티에 들어가 헌혈증서 기부가 필요한 사람들을 본다.
 3. 사연을 보고 자신의 헌혈증서 1개를 기부하기로 결심한다.
 4. 피기부자의 지갑 주소와 기부할 헌혈증서 개수를 입력하고 기부 버튼을 눌러 기부한다.
 5. 생애 첫 헌혈을 하고 기부까지 한 홍길동은 자신을 뿌듯해한다.
 
 #### #3
 *헌혈을 한 달에 한번 하는 직장인 나헌혈은 헌혈 공가를 신청하고자 한다.*
 
 0. 나헌혈은 웹 페이즈를 실행한다.
   0-1. 본인의 개인키로 로그인하여 기관 전용 페이지에 접근한다.
 1. 나헌혈은 e-mail로 회사에게 본인의 개인키를 전달한다.
 2. 나헌혈의 개인키를 받은 회사는 회사 페이지에서 나헌혈의 개인키를 입력하고 나헌혈의 헌혈 기록을 확인한다.
 3. 회사는 나헌혈의 헌혈 기록을 확인하고 헌혈 공가를 부여한다.
 4. 나헌혈은 헌혈 공가를 받고, 앞으로 헌혈을 열심히 해야겠다는 다짐을 한다. 
 
</details>

<details>
 <summary>📈시스템 흐름도</summary>
 
 ### User-case Diagram
 <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226175546-bf2e1f79-ad69-4ae9-a8e0-1696a13b59c5.png"/></p>
 <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226175628-88cf9715-dde5-470b-8b6f-7f27c7d711d6.png"/></p>
 <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226175650-7374eb3e-c222-449d-89f2-91ab102358f0.png"/></p>

 ### Sequence Diagram
  <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226180951-e0b94533-fcae-4952-b2bd-a54c39a2c717.png"/></p>
  <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226181073-91a8ba22-df67-461b-b157-8dd28c832924.png"/></p>
  <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226181220-1ee4ee53-a64f-4ff4-af62-e98f5113d3ba.png"/></p>

 ### Architecture
  <p align='center'><img src="https://user-images.githubusercontent.com/98978787/226175034-a546e12a-463b-4871-b340-9094853670d9.png"/></p>
</details>

## 📔모델링 설명
<p align='center'>
<br>
<div align="center">
 <img width="80%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/e69769f3-5eb2-4472-9bfb-67f5b23b78cb"/>

</div>
</p>

**리츠 주가등락 예측모형에 대한 모델 설계 과정은 다음과 같습니다.**
1. 수집 및 전처리 
2. 변수 선정
3. 모델링
4. 평가 검증 및 성능 측정

### 1. 수집 및 전처리
**데이터 수집**

2019년 1월 ~ 2022년 12월을 기준으로 하여 데이터를 수집하였습니다.
- 각 리츠 일별 / 투자자별 거래 데이터를 한국 주식 거래소(KRX)에서 수집하였습니다.
- 각 리츠 분기별 재무상태표 데이터와 일별 / 월별 거시경제 데이터는 FnGuide를 통해 수집하였습니다.
- 일별 / 부동산 유형별 뉴스 데이터는 빅카인즈를 통해 수집하였습니다.

**파생변수 생성**
- 투자자별 리츠 상품 거래데이터를 통해 "정보비대칭 변수"(기관, 외국인별 순매수도 금액, 체결강도)를 파생변수로 추가하였습니다.
- 일별 주식 거래 데이터를 활용하여 "테크니컬 변수"(SMA20, MACD, ATR, TR, RSI, SLOW_K)를 파생변수로 추가하였습니다.
- 부동산 뉴스테이터를 활용하여 부동산 유형별로 감성 분석을 진행하고 개별리츠의 투자 자산 비중에 맞춰 가중평균한 "부동산 뉴스 심리지수 변수"를 파생변수로 추가하였습니다.


### 2. 변수 선정
**변수 유의성 확인**
앞에서 추출한 후보변수를 고전적 회귀모형 가정(CLM)을 기준으로 변수의 유의성을 확인하였습니다.

- 정규성 검정
정규성 검정 결과 대부분 변수가 정규성을 만족하지 않는다는 것을 확인하였습니다. CLM가정을 중 하나인 정규성을 만족시키기 위해서 데이터 분포의 양 끝단 데이터를 0.5%를 제거하는 윈저라이징 기법을 통해 정규성을 확보하고자 하였습니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/f85a0ab5-1b28-400e-8281-6ccb37b53488"/>

</div>
</p>

 - 다중공선성 확인
상관관계를 파악하기 위해 히트맵으로 변수간 상관의 여부를 파악하고 VIF계수로 그 상관의 정도를 확인하였습니다. 다중공선성이 너무 높은 변수들은 제거하고 모델링을 진행하였습니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/9f8fd758-c54d-4dcd-9115-ea1da9130952"/>

</div>
</p>

이를 통해 모델 학습에 사용 될 최종 변수들을 선정하고 하나의 데이터프레임으로 합쳐 최종 데이터셋을 생성하였습니다. 

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/8fb22b82-3870-4839-b7ad-74eed17485aa"/>

</div>
</p>

종속변수는 한달 뒤 주가등락 여부를 확인하는 것으로 상승, 보합 및 하락으로 이진변수로 구성하였습니다. 종속 변수 분포를 확인한 결과, 1:1 비율로 데이터가 균형있게 존재함을 파악하였습니다. 

### 3. 모델링
**알고리즘 채택**
종속변수 주가 등락을 예측하기 위해 분류 알고리즘을 사용하였습니다. 로지스틱 회귀모형, 트리계열의 XGBoost, CatBoost, 기타 분류 모델인 SVM, Naive Bayes 분류 모형 등의 알고리즘을 사용하여 모델링을 진행한 결과, 트리 기반의 XGBoost 알고리즘이 가장 좋은 성능을 보여주었기 때문에 XGBoost를 채택하였습니다.

### 4. 평가 검증 및 성능 측정
**성능 평가 지표**
모형을 평가함에 있어 분류 모델에서 주로 사용되는 Confusion Matrix를 기반으로 Accuracy, Precision, Recall, F1 score를 측정하였습니다. 
<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/fced78cf-c4c2-491a-a6a5-a39ff006983c"/>

</div>
</p>

**피쳐 중요도**
트리계열 알고리즘에서 어떤 변수가 가장 큰 영향을 미쳤는지 파악하기 위해 학습시킨 모형에서 피쳐중요도를 확인하였습니다. 1달 뒤의 주가등락을 예측하였기 때문에 중장기 주가 등락을 예측할 때 중요한 변수들임을 파악할 수 있습니다. 
<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/2c40566a-2006-495b-937b-11c0faa81d0a"/>

</div>
</p>

## 📔대시보드 설명
### 🩸**SAR Dashboard** ###
웹을 처음 실행 시, 사용자는 우측 상단에 회원가입 버튼을 클릭합니다. 이후 Klaytn Wallet의 개인키를 통해 회원가입을 진행합니다. 

<table>
  <tr>
   <td><img src="https://user-images.githubusercontent.com/96776691/225880429-e796c8a0-f47d-4246-9585-09bbd67f2473.png" height="150" width="300"/></td>
   <td><img src="https://user-images.githubusercontent.com/96776691/225880685-3a21c5e0-8ffc-4865-895e-56fd3d84324b.png" height="150" width="300"/></td>
   <td><img src="https://user-images.githubusercontent.com/96776691/225881263-951e6f3c-78ea-4672-9c52-2f6c17175763.png" height="150" width="300"/></td>
  </tr>
 </table>

 P:LOW서비스의 유저는 "일반유저, 조회기관, 헌혈기관" 총 3가지로 나눌 수 있습니다.


 ### 일반유저
- 최근 헌혈정보 확인
개인키로 로그인 시, 최근 헌혈정보를 확인할 수 있습니다.
<table>
  <tr>
   <td><img src="https://user-images.githubusercontent.com/96776691/225883972-73ee3082-307c-4227-96ae-157fdcf631d0.png" width="400"/></td>
   <td><img src="https://user-images.githubusercontent.com/96776691/225884383-1c2fe716-6260-4135-85fd-8c6bb3d1d657.png" width="400"/></td>
  </tr>
  <tr>
   <td><img src="https://user-images.githubusercontent.com/96776691/225884454-d55a62a9-74d9-4fc0-bd0e-6f744c5c5c2d.png" width="400"/></td>
   <td><img src="https://user-images.githubusercontent.com/96776691/225884540-942fe5a5-dc69-4799-b3e8-f38a8e23bcaa.png" width="400"/></td>
  </tr>
 </table>

- 헌혈 기록 확인
‘내 정보’ 페이지에서 지금까지의 헌혈정보를 확인할 수 있습니다.
 <p align='center'><img src="https://user-images.githubusercontent.com/96776691/225885193-79f03000-1438-4086-802c-9254ff3c925b.png" width="700"/></p>

- 헌혈커뮤니티
P:LOW Web유저들과 헌혈커뮤니티를 이용할 수 있습니다. 헌혈증서가 필요하다는 글을 올릴 수 있고, 타 유저들이 쓴 글을 확인하고 게시글에서 바로 헌혈증서를 기부할 수도 있습니다.
<p align='center'><img src="https://user-images.githubusercontent.com/96776691/225885322-349a28f8-3460-43ca-8e50-40840f2a7328.png" width="700"/></p>

- 헌혈증서 기부
헌혈증서 기부 대상자의 지갑주소, 헌혈증서 기부 개수를 입력하고 ‘기부’버튼을 누르면 헌혈증서를 기부할 수 있습니다.
<p align='center'><img src="https://user-images.githubusercontent.com/96776691/225885500-320c1e6a-f244-483e-b534-f537db56b35c.png" width="700"/></p>

- 기부 내역도 확인할 수 있습니다.
<p align='center'><img src="https://user-images.githubusercontent.com/96776691/225885632-c319a61e-a66c-4450-99f3-c460bfaa31a3.png" width="700"/></p>


### 조회기관
- 조회 기능
조회대상자의 지갑주소와 조회비밀번호를 입력하여 헌혈기록을 조회할 수 있습니다.
<p align='center'><img src="https://user-images.githubusercontent.com/96776691/225885989-62a5bc63-3d21-4c01-b6b3-b6259399f9f0.png" width="700"/></p>

- 조회내역 확인
조회 기능을 사용했을 때 조회대상의 지갑주소 정보, 조회일 정보를 확인할 수 있습니다.
<p align='center'><img src="https://user-images.githubusercontent.com/96776691/225886180-4b870258-23ca-4562-b3f2-f894457769f0.png" width="700"/></p>


### 헌혈기관
- 헌혈증명서 발행
헌혈자의 개인 정보를 입력하고 지갑주소를 입력 후 , ‘발행’버튼을 클릭하면 헌혈증명서가 발행됩니다.

- 헌혈증명서 발급기록 확인
헌혈기관이 발급한 헌혈정보(주민등록번호, 이름, 헌혈분류, 발행일)을 확인할 수 있습니다.
<p align='center'><img src="https://user-images.githubusercontent.com/96776691/225886329-c65639f5-dfd7-4529-b1fa-8f7d844abf74.png" width="700"/></p>


<!--
### 🖥화면 정의
<table>
 <tr>
  <td><img src="https://user-images.githubusercontent.com/40621030/134689804-f72fc601-00cb-462b-a332-a1bcb62ad8a1.png" width="230"/></td>
  <td><img src="https://user-images.githubusercontent.com/40621030/134689811-03fca8d5-26fd-4678-a398-df31655ebae5.png" width="230"/></td>
  <td><img src="https://user-images.githubusercontent.com/40621030/134689813-b89f9162-4e74-48c7-9ac6-57e22f355827.png" width="230"/></td>
 </tr>
 <tr>
  <td><img src="https://user-images.githubusercontent.com/40621030/134689816-4aeb35f6-ca24-4bc4-a4b5-902318b8d895.png" width="230"/></td>
  <td><img src="https://user-images.githubusercontent.com/40621030/134766861-33bf44f8-1330-43d2-91af-4a68f2432507.png" width="230"/></td>
 </tr>
</table>
-->

---

## 컴퓨터 구성 / 필수 조건 안내 (Prerequisites)
* ECMAScript 6 지원 브라우저 사용
* 권장: Google Chrome 버젼 77 이상
* Node.js >= 14
* 0.7.0 < = Solidity <= 0.9.0
* React.js >= 18
* React.router.dom >= 6

---

## 🔨기술 스택 (Technique Used) 
### Server(back-end)
<table>
 <tr>
  <td><a href='https://nodejs.org/ko/'><img src='https://user-images.githubusercontent.com/40621030/136699173-a5a2e626-9161-4e30-85fd-93898671896e.png' height=80/></a></td>
  <td><a href='https://www.mongodb.com/'><img src='https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/MongoDB_Logo.svg/2560px-MongoDB_Logo.svg.png' height=80/></a></td>
  <td><a href='https://ko.docs.klaytn.foundation/content/dapp/sdk/caver-js/getting-started'><img src='https://raw.githubusercontent.com/klaytn/caver-js/HEAD/assets/logo/caver-js.png' width = 200 height=120/></a></td>
 </tr>
 <tr>
  <td align='center'>Node Js</td>
  <td align='center'>MongoDB</td>
  <td align='center'>Caver Js</td>
 </tr>
</table>

<details>
 <summary>MongoDB DDL 설명</summary>
 
 ### MongoDB 데이터베이스 구성
 - Database 명 : BloodChain
 - DB 관리자 명 : Juyeon

 - Post Schema
   - address : 사용자 지갑 주소
   - title : 글 제목
   - content : 글 내용
   - createdAt : 글 작성 날짜
 ```

 Collections.test.datalists
 +----------+-------------+------+-------------------+----------------+
 | Field    | Type        | Null | Default           | Extra          |
 +----------+-------------+------+-------------------+----------------+
 | _Id      | ObjectId    | NO   |                   | auto_created   |
 | address  | String      | NO   | user_address      |                |
 | title    | String      | NO   |                   |                |
 | content  | String      | NO   |                   |                |
 | createdAt| Date        | NO   | CURRENT_TIMESTAMP |                |
 +----------+-------------+------+-------------------+----------------+

 ```

 ***

  *img - Images Handling*

  **POST /img/upload**
  > parameters: {"img_binary":"base64 encoded string","d_num":"string"}   
  > status: 200 -> 204 or 205로 변경 고려   
  > respose: {"status":200,"imd_id":img_id,"user_d_num":d_num}

  **GET /img/output-params/:img_id/:d_num**
  > parameters: {"name": "string", "d_num":"string", "password": "string"}   
  > status: 200   
  > respose: {"status":201,"user_name":name,"msg":'User Created Successful'}
 </details>
 
### Front-end
<table>
 <tr>
  <td align='center'><img src='https://velog.velcdn.com/images/c_10/post/eb16ac48-e413-4fd5-aa9b-ba06f553c4db/image.png' height=80></td>
  <td align='center'><img src='https://blog.kakaocdn.net/dn/bxKpyX/btrhh6XUeBq/sLUMc9vyF6semdllCQJvlK/img.jpg' height=80></td>
 </tr>
 <tr>
  <td align='center'>React JS</td>
  <td align='center'>Bootstrap</td>
 </tr>
</table>
<details>
 <summary>Front-end Description</summary>
 내용채우는중
- [`url_launcher: ^6.0.12`](https://pub.dev/packages/url_launcher)
</details>



### Blockchain
 <table>
 <tr>
  <td><a href="https://solidity-kr.readthedocs.io/ko/latest/"><img src='https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/Solidity_logo.svg/1200px-Solidity_logo.svg.png' height=80></a></td>
  <td><a href="https://ko.docs.klaytn.foundation/"><img src='https://cdn-images-1.medium.com/max/1200/1*3tSS6q_D-lyttNdlRwqoQw.png' height=80></a></td>
  <td><a href="https://trufflesuite.com/"><img src='https://trufflesuite.com/assets/logo.png' height=80></a></td>
  <td><a href="https://remix.ethereum.org/"><img src='https://repository-images.githubusercontent.com/59065830/b62be480-45d2-11ea-9989-803db0f9c44d' height=80></a></td>
  
 </tr>
 <tr>
  <td align='center'>Solidity</td>
  <td align='center'>Klaytn Network</td>
  <td align='center'>Truffle</td>
  <td align='center'>Remix IDE</td>
 </tr>
 </table>
 <details>
 <summary>Blockchain Description</summary>
 
### Why Klaytn?

---
- 풍부한 한국어 Documentations
   > 국내 기업 GroundX가 개발한 블록체인 네트워크로,
   한국어로 잘 정리된 Docs와 튜토리얼
   그리고 활성화되어 있는 포럼 및 커뮤니티를 통해 수월한 개발이 가능했습니다.
  
- Remix 및 Metamask와의 연동성
  > Smart Contract의 작성, 테스트 및 배포에
  용이한 Remix IDE와 Metamask에서
  Klaytn Network와의 연동 환경 제공
  
- 빠른 속도
  > 이전 세대 EVM 계열의 네트워크 보다 
  빠른 TX 속도와 저렴한 TX 수수료
 
# Smart Contract Docs
 ## Structures
  ### Certificate
 - 헌혈증명서 structure로 사용자의 헌혈을 증명할 기본적인 상세정보를 담는다.
 ```Solidity
     struct Certificate {
        string name;
        string id;
        string bloodType;
        string home_address;
        string certificateNum;
        string donateType;
        uint date; // UNIX Time
    }
 ```
 
 ### Donation Certificate
 - 사용자가 기부로 받은 즉 거래를 할 수 없는 헌혈증서로 간단한 정보만을 담는다.
 ```Solidity
     struct DonationCertificate {
        address donate_to;
        uint date;
        uint256 donate_count;
    }
 ```
 
 ## Modifiers
 ### checkDepartment
  - 사용자의 소속을 구분하여 alert
  ```Solidity
    modifier checkDepartment(address _userAddress){
        if(msg.sender == _userAddress){
            require(userDepartment[_userAddress]>0,"Msg Sender's Department Not Set(from modifier)");
        } else{
            require(userDepartment[_userAddress]>0,"User Department Not Set(from modifier)");
        }
        _;
    }
 ```
 
 ### checkAdmin
  - 사용자 Admin Check
  ```Solidity
    modifier checkAdmin(address _userAddress){
        require(_userAddress == deployerAddress,"Msg Sender is Not a Deployer");
        _;
    }
 ```
  
 ## Department Types
 ### code 1 : 일반 유저
 ### code 2 : 일반 기업
 ### code 3 : 공인 헌혈 기관
 
 ## Mapping
 ### certificateOwner
  - 생성된 Certificate Structure(헌혈증명서)의 소유자를 매핑
   ```Solidity
    mapping(uint256 => address) public certificateOwner;
 ```
 ### ownedCerts
  - 사용자가 소유하고 있는 Certificate을 Certificate Array 형태로 매핑
  ```Solidity
     mapping(address => Certificate[]) public ownedCerts;
 ```
 ### departmentMintedRecord
  - 공인된 헌혈 기관의 전자 헌혈 증명서 발급 기록 매핑
  ```Solidity
mapping(address => Certificate[]) private departmentMintedRecord;
 ```
 ### inquiryRecord
  - 일반 기업의 개인 사용자의 헌혈기록 조회시 조회한 기록을 매핑
  ```Solidity
mapping(address => address[]) private inquiryRecord;
 ```
 ### DonationRecord
  - 사용자의 헌혈증서 기부 기록 매핑
   ```Solidity
mapping(address => DonationCertificate[]) private DonationRecord;
 ```
 ### userDepartment
  - 사용자의 소속 기관 매핑
   ```Solidity
mapping(address => uint) private userDepartment;
 ```
 

---
</details>

---

## 💽설치 안내 (Installation Process)
  
  #### 🩸**Canary Web Deployment**
  ```bash
  git clone https://github.com/giirafe/paran_bloodchain.git
  sudo apt-get update
  sudo apt-get install npm 
  cd paran_blockchain
  npm install
  cd frontend
  npm run start
  ```
  
  #### **Remix IDE사용 스마트 컨트랙트 Deployment 시**
  ```Solidity
  pragma solidity >= 0.7.0 <=0.9.0 사이 버젼 Compiler 사용
  ```
  

---

## 📱프로젝트 사용법 (Getting Started)
<!--
**마크다운 문법을 이용하여 자유롭게 기재**

잘 모를 경우
구글 검색 - 마크다운 문법
[https://post.naver.com/viewer/postView.nhn?volumeNo=24627214&memberNo=42458017](https://post.naver.com/viewer/postView.nhn?volumeNo=24627214&memberNo=42458017)

 편한 마크다운 에디터를 찾아서 사용
 샘플 에디터 [https://stackedit.io/app#](https://stackedit.io/app#)
-->

---

## 📈프로젝트 전망

- 리츠 시장의 정보 비대칭성 해소

일반 투자자들은 분산된 리츠의 정보들을 SAR 대시보드를 통해 한눈에 쉽게 파악 가능합니다. 이를 통해 리츠 시장에 대한 정보 비대칭성을 해소하고, 투자자들은 리츠기업의 재정상태, 기초자산의 건전성등을 쉽게 파악해 안전한 투자가 가능해집니다.   

- 리츠 시장의 진입장벽 완화

SAR 대시보드는 투자자들이 알기 어려운 회계용어 및 리츠추천 기능의 원리 등의 정보들에 대해 이해하기 쉬운 설명과 함께 제공됩니다. 각 용어와 원리에 대한 쉬운 설명으로 일반 투자자들의 리츠 투자에 대한 진입장벽이 낮아지고 더 나아가 고령 투자자의 안전한 리츠 투자가 가능해져 퇴직연금 시장의 리츠 투자가 활성화 될 것으로 기대됩니다.  

- 신한투자증권 HTS시스템과 SAR의 연동

SAR이 활성화 되어 신한투자증권에 개설된 연금계좌가 연동되면 투자자들의 더욱 안전한 리츠투자가 가능할 것으로 기대됩니다. 이는 신한투자증권의 연금 운용 활성화 기능으로써 신한투자증권의 IRP계좌를 계설하는 고객들이 많아지고, 더 나아가 리츠 매매가 활성화 될 것으로 예상됩니다. 

- 신한 AI MWS와의 시너지

SAR이 활성화 되면 앞으로 신한 AI, 마켓워닝시스템 'MWS'와의 연계가 가능할 것으로 기대됩니다. 시장에 영향을 많이 받는 부동산의 특성을 고려해 '마켓워닝시스템'을 활용해 리츠 시장에 유연하게 대처하며 적합한 리츠 상품 추천까지 가능한 시스템으로 확장할 것으로 예상됩니다. 

### 🍎개선할 점

- 로그인 절차 간소화

본 서비스에서는 헌혈자, 대한적십자사, 기관(회사)로 사용자가 나누어져 있습니다. 각 사용자들은 본인의 개인키를 이용해 로그인을 하는데 개인키의 길이가 너무 길기 때문에 로그인할 때 불편함이 존재합니다. 따라서 메타마스크와 같은 암호화폐 지갑을 사용하여 로그인 절차를 간소화할 예정입니다. 

- 웹 페이지 UI

현재 웹 페이지 UI는 사용자 친화적이지 않습니다. 특히 헌혈증서 커뮤니티의 UI를 기부자와 피기부자가 이용하기 편리하도록 개선할 필요가 있습니다. 

- 어플리케이션 개발

P:LOW 서비스는 웹 페이지로 개발되었습니다. 헌혈자는 헌혈을 하고 나와 보통 핸드폰의 어플리케이션을 이용하기 때문에 P:LOW 서비스 어플리케이션을 개발하여 헌혈자가 보다 이용하기 편하도록 할 예정입니다. 


---

## 🕋팀 정보 (Team Information)

과학 기술이 발전해도 사람의 혈액을 대체할 수 있는 것은 발명되지 않았습니다.  
피를 나누는 것은 생명을 살리는 고귀한 행동이며 가치 있는 일입니다.  
저희는 **헌혈 활성화**라는 공공의 이익을 위해 뭉쳤습니다.  

안녕하십니까, 헌혈로 세상의 가치를 잇다.  
저희는 블러드 체인팀입니다. 

<table>
 <tr>
  <td></td>
  <td>Name</td>
  <td>Role</td>
  <td>github</td>
  <td>e-mail</td>
 </tr>
   
 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/76638529?v=4" width="50" height="50"></td>
  <td align='center'>June Seo</td>
  <td align='center'>Back-End / Smart Contract</td>
  <td align='center'><a href="https://github.com/giirafe"><img src="http://img.shields.io/badge/giirafe-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:seojune408@gmail.com"><img src="https://img.shields.io/badge/seojune408@gmail.com-green?logo=gmail&style=social"/></a></td>
 </tr>
 
 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/96776691?v=4" width="50" height="50"></td>
  <td align='center'>CheonHa Kim</td>
  <td align='center'>Back-End</td>
  <td align='center'><a href="https://github.com/KimUnderTheSky"><img src="http://img.shields.io/badge/KimUnderTheSky-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:cjsksla@ajou.ac.kr"><img src="https://img.shields.io/badge/cjsksla@ajou.ac.kr-green?logo=gmail&style=social"/></a></td>
 </tr>

 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/87919319?v=4" width="50" height="50"></td>
  <td align='center'>SeongWoo Park</td>
  <td align='center'>Front-End / Design</td>
  <td align='center'><a href="https://github.com/ssongssong00"><img src="http://img.shields.io/badge/ssongssong00-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:seongwoo1205@gmail.com"><img src="https://img.shields.io/badge/seongwoo1205@gmail.com-green?logo=gmail&style=social"/></a></td>
 </tr>

 <tr>
  <td align='center'><img src="https://user-images.githubusercontent.com/98978787/226175108-63792c9b-1d80-45f9-958c-b1d2824f64f1.png" width="50" height="50"></td>
  <td align='center'>Juyeon Lee</td>
  <td align='center'>Front-End / DB for Community</td>
  <td align='center'><a href="https://github.com/Juyeori"><img src="http://img.shields.io/badge/Juyeori-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:dlwndus0728@ajou.ac.kr"><img src="https://img.shields.io/badge/dlwndus0728@ajou.ac.kr-green?logo=gmail&style=social"/></a></td>
 </tr>
</table>

---

## 개발 및 협업 플랫폼

<table>
 <tr>
  <td align='center'><a href="https://github.com/"><img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" height=80/></a></td>
  <td align='center'><a href="https://meet.google.com/"><img src="https://user-images.githubusercontent.com/86545225/137439170-9500c5b2-c47a-4ecc-b588-8c0b14e0eb3b.png" height=80/></a></td>
   <td align='center'><a href="https://www.notion.so/ko-kr"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/Notion-logo.svg/1024px-Notion-logo.svg.png" height=80/></a></td>
 </tr>
 
 <tr>
  <td align='center'>Github</td>
  <td align='center'>Google meet</td>
  <td align='center'>Notion</td>
 </tr>
 
 <tr>
  <td align='center'><a href="https://aws.amazon.com/ko/free/?trk=fa2d6ba3-df80-4d24-a453-bf30ad163af9&sc_channel=ps&s_kwcid=AL!4422!3!563761819834!e!!g!!aws&ef_id=CjwKCAjw5dqgBhBNEiwA7PryaHEPioZu9x8OMoL3DTT7vpN6G6sPP5QORNgE_ajU3-1qu1C3FSKctxoCMqwQAvD_BwE:G:s&s_kwcid=AL!4422!3!563761819834!e!!g!!aws&all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=*all"><img src="https://images.velog.io/images/nari120/post/b14b4105-a561-4cc3-bc9f-87a5ee4eb1b6/aws.png" height=80/></a></td>
  <td align='center'><a href="https://slack.com/"><img src="https://user-images.githubusercontent.com/86545225/137576768-7b07ae82-ea9c-4768-ac5b-5d1f854a2815.jpg" height=80/></a></td>
  <td align='center'><a href="https://zoom.us/"><img src="https://user-images.githubusercontent.com/86545225/137440645-636a8078-208b-4542-bbfd-2823f0572e1c.png" height=80/></a></td>
 </tr>
 
 <tr>
  <td align='center'>AWS</td>
  <td align='center'>Slack</td>
  <td align='center'>Zoom</td>
 </tr>

   
</table>
 


## 저작권 및 사용권 정보 (Copyleft / End User License)
 * [GNU GPL v3](https://github.com/osamhack2021/AI_APP_WEB_Canary_Canary/blob/main/LICENSE)

This project is licensed under the terms of the GNU GPLv3 license.
  
  ### GPL 선택이유
