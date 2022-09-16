# pytorch를 활용한 딥러닝 입문 
https://www.notion.so/PyTorch-217004801d1447e08f73aa821f605624

# PyTorch 기초
  1. [PyTorch 패키지 기본 구성](https://github.com/jinsusong/study-pytorch-DL/blob/main/PyTorch_%ED%8C%A8%ED%82%A4%EC%A7%80%EC%9D%98_%EA%B8%B0%EB%B3%B8_%EA%B5%AC%EC%84%B1.ipynb)
  2. [텐서 조작 Part1](https://www.notion.so/Part-1-21f76800fef7420cb9d8c55ee20acacd)
  3. [텐서 조작 Part2](https://www.notion.so/Part-2-1c11569b49c846f88c5ae2dc3dc9ddbe)
  4. [파이썬 클래스 Class](https://www.notion.so/Class-39e03d48daa94bc3ab6534d79f0ffba4)
  5. [선형 회귀 (Linear Regression)](https://www.notion.so/Linear-Regression-f14cba06943a4730ba2b3fbd9c1dddd5)
      - Code : Linear Regression[Link](https://github.com/jinsusong/study-pytorch-DL/blob/main/PyTorch%EB%A1%9C_%EC%84%A0%ED%98%95%ED%9A%8C%EA%B7%80_%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0.ipynb) 
      - 자동 미분 (Autograd)[Link](https://www.notion.so/Autograd-89e8b322812049e3958caadf3a1e368a)
      - 다중 선형 회귀(Multivariable Linear regression)[Link](https://www.notion.so/Multivariable-Linear-regression-3334f468a5404e318d595408cb0f1fe8)
      - nn.Module로 구현하는 선형 회귀[Link](https://www.notion.so/nn-Module-0db58f18fc634fd79d14fd9db6fafac7)
      - 클래스로 파이토치 모델 구현[Link](https://www.notion.so/74a771bad7a94c43ae556815905db5f1)
      - 미니 배치와 데이터 로드[Link](https://www.notion.so/b8f0f343f50b42bfb98f235e760086b5)
  6. [로지스틱 회귀 (Logistic Regression](https://www.notion.so/899974ee39ce4fa0a82a563dfd7d78b3)
      - 로지스틱 회귀[Link](https://www.notion.so/899974ee39ce4fa0a82a563dfd7d78b3)
      - nn.Module[Link](https://www.notion.so/nn-Module-472b2f7c19114c26ae90f0ab954d7766)
      - 클래스로 로지스틱 모델 구현[Link](https://www.notion.so/d43048d2c1534b92910947409a45df30)
  7. [진행중.소프트맥스 회귀](https://www.notion.so/899974ee39ce4fa0a82a563dfd7d78b3)
      - 원-핫 인코딩[Link](https://www.notion.so/a292e7fe82b14a5ab456762d5d6d6f3c)
      - 소프트맥스 회귀[Link](https://www.notion.so/e65b925942ea4d56aaf78d3d4e460bdc)


# 코드 분석 
* Dataset and TensorDataSet : 배치 관련 담당, X,Y 데이터셋을 텐서 형태로 묶음
* Reproductibility : 동일한 데이터와 모델로 학습을 진행했을 때 매번 다른 학습 파라미터가 생성되지 않도록 조정하는거 
* model.eval() : 학습할때만 필요한 Dropout, batchnorm 등을 비활성화 
* torch.no_grad() : 자동으로 Gradient를 계산해주는 Context를 
