# Factor Modeling : Discoverying alpha by using new factor

![Static Badge](https://img.shields.io/badge/project-KHU-<color>)
![Static Badge](https://img.shields.io/badge/version-1.0.0-informational)
![Static Badge](https://img.shields.io/badge/python-3.9|3.10-lightblue)

> 2023학년도 2학기 경희대학교 금융데이터분석 프로젝트 입니다.

## 🚀 프로젝트 소개

> 본 프로젝트는 S&P500 & KAIST & UNIST & KYUNGHEE 퀀트 투자 모델 경진대회에서 제공된 S&P500 데이터를 사용하였습니다.

본 프로젝트는 제공된 데이터를 최대한 활용하고자 하였으며 다양한 데이터셋으로부터 새로운 팩터를 찾고 이 팩터를 활용하여
알파를 찾는 "팩터 모델링"과 "팩터 투자"를 진행하였습니다. 

<br/>

## 📌 프로젝트 구성

프로젝트는 크게 팩터 모델링과 팩터 투자 및 백테스팅으로 두 파트로 나눌 수 있습니다.

우선 팩터의 경우, 시장 전체보다는 특정 섹터가 더 높은 설명력을 보일 것이라 판단하여 결측치가 제일 적은 바이오 섹터에서만 국한하여 진행하였습니다.

팩터 모델링에서는 재무, 추정치, 마켓 데이터를 활용하였으며 팩터의 설명력에 대한 검증은 섹터를 설명하는 포트폴리오의 일별 수익률과 
개별 기업간의 일별 수익률의 OLS를 통해 전체 바이오 기업 수 대비 X% 이상의 비율로 P-value가 0.05이하로 나오면 유의미하다고 판단하였습니다. 

재무 데이터와 추정치 데이터 셋의 경우 데이터의 구성과 결측치 비율 등 다양한 부분에서 차이를 보여 팩터 모델링에 대한 파이프라인을 따로 구축하였고, 
통합하여 검증하기 위한 백테스팅 파이프라인과 최종적으로 얻은 멀티 팩터에 대한 포트폴리오와 바이오 섹터 ETF의 수익률 비교하는 팩터 투자에 대한 부분을 구현하였습니다.

![image](https://github.com/khuda-4th/KHUDA_FN_Factor_Modeling/assets/59081655/31ee9d40-b4f0-4404-9255-2f77a984e764)

