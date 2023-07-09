# SAR : 리츠투자플랫폼 

<p align='center'>
<br>
<div align="center">
 <img width="80%" src="https://github.com/ssongssong00/ShinhanAI/assets/87919319/e6783a9a-8838-4732-ab3c-55de0e803af8"/>

</div>

</p>

SAR은 리츠 투자자의 리츠 가치평가를 돕는 대시보드로 
* 한 달뒤 상장 리츠 주가 등락 예측 모델과, 
* 대안 정보를 활용한 대시보드를 통해,
* 리츠 활성화에 기여하고자 합니다.

## 🗂️프로젝트 소개
본 프로젝트는 상장리츠 대시보드와 주가예측 등락 모델을 통해,  
* 리츠 회사와 일반 투자자간 **정보비대칭을 해소**하고,
* 리츠 회사의 **배당수익률 단편 정보의 문제를 해결**하고.
* 리츠의 전반적인 특성(회계, 부동산 정보)를 고려한 주가등락예측 모형으로 **예측 정보**를 제공해
* 궁극적으로 투자자들이 **신중하고 현명한 투자를**하는 것에 목표를 둡니다.

--- 

## 📃주제 정의 문서
 
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

 ---
 
 ## 🗒사용자 정의 문서
 
 ### 페르소나
 <div align="center">
 <img width="80%" src="https://github.com/ssongssong00/ShinhanAI/assets/87919319/816c5bec-1060-4a7f-9c69-87f04cca6680"/>
</div>

 <div align="center">
 <img width="80%" src="https://github.com/ssongssong00/ShinhanAI/assets/87919319/f56f7800-304b-4a20-aa22-85d74e6978d8"/>
</div>

 ### 시나리오
 
 #### #1
 *대기업 은퇴 예정자인 박리츠는 SAR을 통해 은퇴설계에 도움을 얻고자 한다.*
 
 0. 박리츠는 SAR을 실행한다.
 1. 박리츠는 AI 기반 리츠 추천 종목을 확인한다.
 2. 한 달뒤 상승으로 예측된 리츠의 자세한 정보를 확인하기 위해 회계정보 대시보드를 클릭한다.
 3. 해당 리츠가 배당을 꾸준히 주고 있는지, FFO와 같은 주요 지표를 확인한다.
 4. 정리된 투자보고서와 영업보고서를 정독하여 해당 리츠의 재정 상태가 정상인지 확인한다.
 5. 해당 리츠의 기초자산이 건전한지 파악하기 위해 기초자산 대시보드를 클릭한다.
 6. 보유하고 있는 리츠의 기초자산의 유형을 확인하고 투자 시기기 적절한지 파악한다.
 7. 교통, 유동인구 등 대안정보를 활용하여 리츠의 가치 평가에 도움을 얻는다.

---
 
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

---

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


---

## 🕋팀 정보 (Team Information)

안녕하십니까, 저희는 영앤리츠팀입니다. 

<table>
 <tr>
  <td></td>
  <td>Name</td>
  <td>Role</td>
  <td>github</td>
  <td>e-mail</td>
 </tr>

 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/87919319?v=4" width="50" height="50"></td>
  <td align='center'>SeongWoo Park</td>
  <td align='center'>Modeling / Dashboard</td>
  <td align='center'><a href="https://github.com/ssongssong00"><img src="http://img.shields.io/badge/ssongssong00-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:seongwoo1205@gmail.com"><img src="https://img.shields.io/badge/seongwoo1205@gmail.com-green?logo=gmail&style=social"/></a></td>
 </tr>
 
 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/96776691?v=4" width="50" height="50"></td>
  <td align='center'>CheonHa Kim</td>
  <td align='center'>Modeling / Dashboard</td>
  <td align='center'><a href="https://github.com/KimUnderTheSky"><img src="http://img.shields.io/badge/KimUnderTheSky-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:cjsksla@ajou.ac.kr"><img src="https://img.shields.io/badge/cjsksla@ajou.ac.kr-green?logo=gmail&style=social"/></a></td>
 </tr>
 
 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/76638529?v=4" width="50" height="50"></td>
  <td align='center'>조국</td>
  <td align='center'>Modeling / Dashboard</td>
  <td align='center'><a href="https://github.com/giirafe"><img src="http://img.shields.io/badge/giirafe-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:seojune408@gmail.com"><img src="https://img.shields.io/badge/seojune408@gmail.com-green?logo=gmail&style=social"/></a></td>
 </tr>

 <tr>
  <td align='center'><img src="https://avatars.githubusercontent.com/u/87919319?v=4" width="50" height="50"></td>
  <td align='center'>신은주</td>
  <td align='center'>Modeling / Dashboard</td>
  <td align='center'><a href="https://github.com/tlsdmswn01"><img src="http://img.shields.io/badge/tlsdmswn01-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:seongwoo1205@gmail.com"><img src="https://img.shields.io/badge/seongwoo1205@gmail.com-green?logo=gmail&style=social"/></a></td>
 </tr>

 <tr>
  <td align='center'><img src="https://user-images.githubusercontent.com/98978787/226175108-63792c9b-1d80-45f9-958c-b1d2824f64f1.png" width="50" height="50"></td>
  <td align='center'>이다은</td>
  <td align='center'>Modeling / Dashboard</td>
  <td align='center'><a href="https://github.com/Juyeori"><img src="http://img.shields.io/badge/Juyeori-green?style=social&logo=github"/></a></td>
  <td align='center'><a href="mailto:dlwndus0728@ajou.ac.kr"><img src="https://img.shields.io/badge/dlwndus0728@ajou.ac.kr-green?logo=gmail&style=social"/></a></td>
 </tr>
</table>

---

