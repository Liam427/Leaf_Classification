### 프로젝트 개괄

* 프로젝트에서 사용하는 총 데이터의 수는 약 40000개이고, 각 클래스의 이름은 작물의 종류와 질병 종류를 나타냅니다. 질병 이름이 'healthy'인 경우는 해당 작물이 건강함을 의미합니다. 예를 들어 Potato의 경우 세 가지 클래스 Potato_Early_blight, Potato_Late_blight, Potato_healthy로 분류 됩니다. 이 중에서 Potato_healthy로 분류된 경우가 질병이 없는 Potato를 의미합니다.

### 베이스라인 모델 설계
* 베이스라인 이므로 복잡하게 하지 않게 하였고 아래와 같이 3개의 convolution, 1개의 pooling, 2개의 fully connected layers로 총 6개의 layers로 모델을 설계했습니다.  
![basemodel](https://github.com/Liam427/Leaf_Classification/blob/master/image/basemodel.png)   

### 베이스라인 모델 성능
* 아주 간단한 모델이지만 아래와 같이 높은 성능을 보여 주었습니다.  
![accuracy](https://github.com/Liam427/Leaf_Classification/blob/master/image/basemodel_accuracy.png)

### 베이스라인 모델 test 성능
![test](https://github.com/Liam427/Leaf_Classification/blob/master/image/baseline_test.png)

### 베이스라인 평가
* train, val, test set 간의 차이가 크지 않은 것으로 보아 overfitting의 위험성은 없다고 볼 수 있습니다.  
  또한 test set의 성능이 93%로 높게 나오는걸 알 수 있습니다.

---

### ResNet50 모델 설계
* pytorch에서 제공하는 model 패키지에 있는 resnet50을 이용하여 모델을 설계하였습니다.

### ResNet50 모델 성능
![train](https://github.com/Liam427/Leaf_Classification/blob/master/image/resnet501.png)

### ResNet50 모델 test 성능
![test](https://github.com/Liam427/Leaf_Classification/blob/master/image/resnet50_test.png)
