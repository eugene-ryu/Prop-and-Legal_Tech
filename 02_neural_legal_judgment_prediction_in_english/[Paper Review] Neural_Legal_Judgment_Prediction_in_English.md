![Neural Legal Judgment Prediction in English](./imgs/judge_predict_header.png)

## Abstract<br>
European Court of Human Rights 데이터셋을 포함한, 영어로된 (머신러닝용) 새로운 데이터셋을 선보인다.<br>
이 데이터셋을 가지고 여러가지 모델들을 테스트해보았으며, 세 종류의 태스크에 대해서 이전의 feature-based models(피쳐 베이스 모델들)를 넘어서는 베이스라인(모델)을 제시한다.<br><br>

## Legal Prediction Tasks<br>
(1) binary violation classification - 침해 사건에 대한 이진 분류<br>
- 사람의 어떤 기본권이라도 "침해를 했는가"(violated), 침해하지 "않았는가"(not violated)<br><br>
(2) multi-label classification - 여러 레이블 분류<br>
- 사람의 "어떤" 기본권이나 프로토콜을 침해했는가를 체크하며, 레이블이 없는 것은 침해하지 않았다는 뜻이다<br><br>
(3) case importance prediction - 케이스 중요도 예측<br>
- 사건의 중요도를 1(중요), 2(덜 중요), 3(보통), 4(중요하지 않음)로 나누어서 체크했다<br><br>


## Neural Models<br>
### BiGRU-Att<br><br>

### HAN (Hierarchical Attention Network)<br><br>

### LWAN (The Label-Wise Attention Network)<br><br>

### BERT and HIER-BERT<br><br>