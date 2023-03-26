![A Multi-Task Benchmark for Korean Legal Language Understanding and Judgement Prediction](./imgs/benchmark_paper_header.png)<br>
paper: https://arxiv.org/pdf/2206.05224.pdf<br><br><br>

## Abstract <br>
법률 인공지능에 사용할 수 있는 한국어 법률 데이터셋인 LBOX OPEN과 한국어 법률 자연어처리 모델인 LCUBE를 공개한다.<br><br>

https://github.com/lbox-kr/lbox-open<br><br><br>


## Introduction<br>
엘박스 오픈(LBOX OPEN) 데이터셋은 아래처럼 구성되어 있다<br><br>

1) 하나의 법률 용어집(PRECEDENT CORPUS/ one legal corpus): 근 44년간의 147k 한국 판례 모음 (259M개의 토큰들)<br><br>

2) 두 개의 분류 태스크(two classification tasks)<br>
    2-1) 사건 이름 분류(CASE NAME / case names), 11.3k의 facts와 case name 페어<br>
    2-2) 법령 예측(STATUTE / statutes preediction), 2.8k의 facts와 거기에 상응하는 법령들<br><br>
    
3) 두 개의 법률 판결 예측(two legal judgement predictions, LJP)<br>
    3-1) 벌금 액수/노역형/노역이 없는 수감형을 예측하는, 10.5k 범죄 샘플들 (LJP-CRIMINAL)<br>
    3-2) 구제 정추(claim for relief)와 사실들이 input, 주장을 받아들이는 정도를 output으로 하는, 4.7k 민사 샘플들(LJP-CIVIL)<br><br>
    
4) 하나의 요약 태스크(one summarization task)<br>
    4-1) 대법원 판례들과 이에 상응하는 요약본들, 20k (SUMMARIZATION)<br><br>
    
또한, 케이스에서 드문 케이스 카테고리들에 대한 데이터들(CASE NAME+, 31k 샘플), 법령 분류 태스크들(STATUTE+, 17.7k 샘플), 요약 태스크에서의 긴 인풋 시퀀스들(SUMMARIZATION+, 51k 샘플)들도 포함시켰다.<br><br> 


이 엘박스 오픈 데이터셋을 사용해서 사전 학습을 시킨, 첫번째 한국어 법률 언어 모델인 엘큐브(LCUBE)도 발표한다.<br>
GPT2에 기초한 encoder-only 모델로, text classification 문제에서 m5(encoder-decoder LM)와 경쟁해볼만한 성과를 이뤘으나, summarization 태스크에서는 엘큐브가 다른 모델들 대비 특별한 이점을 보이지 못했다.<br><br><br>


## Background<br>
#### Korean Legal System<br>



