# Domain-Robust-Retraining-of-Pretrained-Language-Model

  * 한국어에 대한 많은 PLM(Pretrained Language Model)들이 있지만, 대부분 문어체에 대한 PLM이 존재합니다. 여기서는 한국어 대화(구어체) 데이터의 예측을 위한 재학습된 PLM을 소개합니다.
  * 이 모델은 [klue/roberta-base](https://huggingface.co/klue/roberta-base?text=%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%EC%9D%98+%EC%88%98%EB%8F%84%EB%8A%94+%5BMASK%5D+%EC%9E%85%EB%8B%88%EB%8B%A4.)를 기본 모델로 삼고 구어체 데이터셋을 추가적으로 Retraining을 시킨 것으로, 우리는 이를 Kconvo-roberta로 정의합니다.
  * 재학습시킨 데이터셋은 [국립국어원](https://corpus.korean.go.kr/request/corpusRegist.do) 및 [AI-Hub](https://www.aihub.or.kr/aihubdata/data/list.do?pageIndex=1&currMenu=115&topMenu=100&dataSetSn=&srchdataClCode=DATACL001&srchOrder=&SrchdataClCode=DATACL002&searchKeyword=&srchDataRealmCode=REALM002&srchDataTy=DATA003)을 통해 수집하였으며, 수집한 데이터셋은 아래와 같습니다.

    * 국립국어원

         * 온라인 대화 말뭉치 2021
         * 일상 대화 말뭉치 2020
         * 구어 말뭉치
         * 메신저 말뭉치

    * AI-Hub
  
         * 온라인 구어체 말뭉치 데이터
         * 한국어 음성
         * 자유대화 음성(일반남여)
         * 한국어 대화
         * 한국인 대화음성
         * 감성 대화 말뭉치
         * 주제별 텍스트 일상 대화 데이터
         * 용도별 목적대화 데이터
         * 한국어 SNS
         
-----------------------------------------------------------------
## Motivation

 * 연구 과제
   * 소셜네트워크에서의 온라인그루밍 위험성 자가탐지 기술 개발
 * 연구 목적
   * 구축된 한국어 온라인 그루밍에 관련 대화 텍스트의 대화 분석&의미 분석 예측에 대한 Performance Upgrade
 * 연구 결과
   * 한국어 온라인 그루밍 데이터셋, 온라인 그루밍 대화 분석에 특화된 PLM
 
-----------------------------------------------------------------
## Paper



 * [Don't Stop Pretraining: Adapt Language Models to Domains and Tasks](https://aclanthology.org/2020.acl-main.740/)
 
-----------------------------------------------------------------
## Contributor

 * `Tak-Sung Heo`, `Yeongjoon Park`, `Byeong-Cheol Jo`
