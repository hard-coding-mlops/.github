# Hard Coding MLOps
## KoBERT 기반 뉴스 토픽 분류 학습 모델 MLOps

![mini_mlops_main](https://github.com/hard-coding-mlops/mini-mlops-fastapi/assets/111658806/daaec923-9454-4431-8270-350465041c0e)

<!-- font weight bold -->
<div align="center">
서경 SW 아카데미 <span style="font-weight:bold; font-size:1.2rem">Team "Hard Coding"</span> with Hecto Innovation
</div>

## 🤔 MLOps 개발 배경
뉴스 기사 분류 모델을 운영하는 과정에서 사용자에게 향상된 성능의 모델을 제공하고자 할 때, 새로운 데이터를 수집하고, 이를 정제하고, 모델을 학습시키고, 평가하고, 배포하는 과정을 반복하였습니다.

이러한 과정을 직접 수행하다보니, 모델 개발에 집중하기 어려웠으며, 중간에 휴먼 에러가 발생하여 특정 과정을 다시 수행하며 시간을 많이 소모하게 되었습니다.

기존의 방식은 반복적이고, 비효율적이며, 사용자에게 향상된 성능의 모델을 제공하기 이전에 안전하지 못한 운영 환경을 제공하는 것은 위험하다고 판단하여, 반복적인 작업을 자동화하고 안정적인 운영을 하고자 했습니다.

## 📚 기술 스텍
| 분류 | 기술 |
|:-:|:-:|
| <span style="font-weight:bold">Back-End</span> | <img src="https://img.shields.io/badge/FastAPI-141414.svg?style=for-the-badge&logo=fastapi&logoColor=009688" /> <img src="https://img.shields.io/badge/Colab-141414.svg?style=for-the-badge&logo=googlecolab&logoColor=F9AB00" />|
| <span style="font-weight:bold">Front-End</span> |<img src="https://img.shields.io/badge/React-141414.svg?style=for-the-badge&logo=react&logoColor=61DAFB" /> <img src="https://img.shields.io/badge/Redux-141414.svg?style=for-the-badge&logo=redux&logoColor=764ABC" />|
| <span style="font-weight:bold">Database</span> |<img src="https://img.shields.io/badge/MySQL-141414.svg?style=for-the-badge&logo=mysql&logoColor=4479A1" /> <img src="https://img.shields.io/badge/Amazon RDS-141414.svg?style=for-the-badge&logo=amazonrds&logoColor=527FFF" />|
| <span style="font-weight:bold">Deployment</span> |<img src="https://img.shields.io/badge/ngrok-141414.svg?style=for-the-badge&logo=ngrok&logoColor=1F1E37" /> <img src="https://img.shields.io/badge/KT_Cloud-KT_Cloud?style=for-the-badge&color=%231ae4ee" style="height:1.98rem">|
| <span style="font-weight:bold">Design</span> |<img src="https://img.shields.io/badge/Figma-141414.svg?style=for-the-badge&logo=figma&logoColor=F24E1E" />|


## 🛠️ 주요 기능
* 회원 관리  
카카오 기반 OAuth 인증과 JWT 토큰을 활용하여 관리자 페이지 접근

* 뉴스 기사 수집 자동화  
다음 뉴스에서 각 분야별로 한 페이지씩 수집

* 기사 정제 및 전처리 자동화  
정제를 통해 수집된 기사 중 짧은 기사, 영문 기사, 중복 기사를 적절히 처리 및 삭제하고, 학습 과정에서는 알맞는 형태로 토큰화 진행

* 모델 학습 및 파라미터 조정  
관리자가 설정한 파라미터 값과 특정 양(범위)의 정제 데이터를 학습

* 모델 저장 및 버전 관리  
학습된 모델은 파일로 저장하고 관리자 페이지에서 관리

* 모델 테스트, 평가 및 배포 여부 결정  
학습된 모델을 테스트하고 평가하며, 사용자 서비스에 배포할 지 결정

* 서비스 모델 모니터링  
배포된 모델에 대한 주요 정보와 사용자 접근성을 모니터링

- 기사 분야 예측 서비스 (사용자 페이지)


## 📆 프로젝트 기간
2023.11.06 ~ 2023.12.26

## 🏗️ 시스템 아키텍처
<img alt="HARD_CODING_MLOPS_SYSTEM_ARCHITECTURE" src="https://github.com/user-attachments/assets/dbd42a86-e491-4f26-a7aa-f25a9f1f056a" width="100%">

## 🗃️ DB 설계
![mini_mlops_db](https://github.com/hard-coding-mlops/mini-mlops-fastapi/assets/111658806/3a3b0172-1e71-4e65-9831-3d578b2bec27)
