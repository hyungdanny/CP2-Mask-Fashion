# 2 stage Object Dectection for new duplicate image detection

## Index
  - [프로젝트 정의](#프로젝트정의) 
  - [데이터셋 설명](#데이터셋설명)
  - [진행과정](#진행과정)
  - [진행 도중 발생한 문제점과 그 해결 과정](#진행도중발생한문제점과그해결과정)
  - [결과물](#결과물)
  - [한계점과 해결방안](#한계점과해결방안)


#### 이 프로젝트에 대하여
<!--Wirte one paragraph of project description -->  
 - 이 프로젝트는 코드스테이츠 AI 부트캠프 10기 과정을 수료하기위해 진행한 마지막 프로젝트입니다.
 - 컴퓨터비젼 분야에 관심을 갖게 되어 이 분야를 좀 더 깊게 탐구하기 위하여 프로젝트를 기획했습니다.
 - 2stage 탐지모델의 대표인 R-CNN 계열 모델을 시초부터 최신 모델을 구축하면서 어떤 문제점을 개선하면서 발전해왔는지 직접 확인하는 것이 목표입니다.
 - 데이터는 DeepFashion2를 선정하였고 이유는 Annotaion이 잘 되어있고 연구자가 패션에 관심이 있기 때문입니다.
 - 주목할 점은 같은 데이터를 사용하되 다른 모델을 적용시키면서 성능이 얼마나 개선이 되고 어떤 차이를 가지는 지 확인하는 것입니다. 

*****

## 프로젝트 정의 
1. 문제 정의 : 여러 상황에서 촬영된 이미지따라 동일한 사물이지만 다른 사물로 인식하는 오류를 개선한다. 
2. 데이터 : DeepFashion2
3. 기대하는 결과값 : 서로 다른 사진이지만 동일한 물건이라는 것을 탐지.
4. 프로젝트 의도 : 2stage 모델 중 R-CNN 부터 차례대로 등장한 모델을 최신 모델까지 구현한다. </br> 
   먼저 모델이 개선될 때 어떻게 성능이 달라지는 지 공부하고 최종 모델에서 어떻게 해야 주어진 문제를 해결할 방안을 찾는다.
5. 성과 지표 : 상위모델을 적용할 때마다 그 이전모델의 성능이 베이스라인이 되어 성과 지표가 된다.


## 데이터셋설명 
1. 데이터 출처 : </br>
@article{DeepFashion2,
  author = {Yuying Ge and Ruimao Zhang and Lingyun Wu and Xiaogang Wang and Xiaoou Tang and Ping Luo},
  title={A Versatile Benchmark for Detection, Pose Estimation, Segmentation and Re-Identification of Clothing Images},
  journal={CVPR},
  year={2019}
}
2. 데이터 수량 : 13가지 옷 종류별 491K, 총 801K개
3. 이미지 설명: 동일한 의류제품을 소비자와 판매자가 촬영한 사진이 ID로 연결되어 있다.
4. Annotation : style, bounding_box, landmarks, segmentation, scale, occlusion, zoom_in, viewpoint 

## 진행과정
*각각 모델별로 폴더가 준비되어 있습니다.*
- [x] R-CNN 모델
- [x] Fast R-CNN
- [ ] Faster R-CNN
- [ ] RPN
- [ ] Mask R-CNN
- [ ] Dectectron
- [ ] Dectectron2

## 진행 도중 발생한 문제점과 그 해결 과정


## 결과물


## 한계점과 해결방안
