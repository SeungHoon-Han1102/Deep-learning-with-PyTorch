# 파이토치 패키지의 기본 구성  


공부해야 할 용어: 네임스페이스, 콘텍스트 매니저, 자체미분가능함수, 유틸리티함수, ONNX

---
1. torch  
- 메인 네임스페이스.  
- 텐서 등의 다양한 수학 함수를 포함.  
- Numpy와 유사한 구조. 
---
2. torch.autogard  
- 자동 미분을 위함 함수들을 포함.  
- 자동 미분의 on/off를 제어하는 콘텍스트 매니저(enable_grad/no_grad), 자체 미분 가능 함수를 정의할 때 사용하는 기반 클래스인 'Function'등이 포함.  
---
3. torch.nn  
- 신경망을 구축하기 위한 다양한 데이터 구조나 레이어 등을 포함.  
- 예시) RNN, LSTM과 같은 레이어 / ReLU와 같은 활성화 함수, MSELoss와 같은 손실 함수  
---
4. torch.optim  
- 확률적 경사 하강법(SGD)를 중심으로 한 파라미터 최적화 알고리즘이 구현되어 있음.   
---
5. torch.utils.data  
- SGD의 반복 연산을 실행할 때 사용하는 미니 배치용 유틸리티 함수가 포함.  
---
6. torch.onnx  
- ONNX(Open Neural Network Exchange)의 포맷으로 모델을 익스포트(export)할 때 사용.  
- ONNX는 서로 다른 딥러닝 프레임워크 간에 모델을 공유할 때 사용하는 포맷.
---
