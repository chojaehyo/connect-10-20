# [P stage1 : Image Classification] 일석CV조
<img width="1085" alt="스크린샷 2022-11-11 오후 1 13 32" src="https://user-images.githubusercontent.com/69153087/201261752-33f6bb6d-ddd0-46fa-a32b-f510c50e5a89.png">

## Member 
<table>
  <tr height="125px">
    <td align="center" width="120px">
      <a href="">김종해_T4047</a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/youngjun04">_</a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/thlee00">_</a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/chojaehyo">_</a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/jphan32">_</a>
    </td>
  </tr>
</table>

**김종해** [T4047] [@Jejugamguel](https://github.com/Jejugamguel) <br/>
**유영준** [T4136] [@youngjun04](https://github.com/youngjun04) <br/>
**이태희** [T4172] [@thlee00](https://github.com/thlee00) <br/>
**조재효** [T4214] [@chojaehyo](https://github.com/chojaehyo) <br/>
**한상준** [T4226] [@jphan32](https://github.com/jphan32) <br/>

## Overview

COVID-19의 확산으로 우리나라는 물론 전 세계 사람들은 경제적, 생산적인 활동에 많은 제약을 가지게 되었습니다. 우리나라는 COVID-19 확산 방지를 위해 사회적 거리 두기를 단계적으로 시행하는 등의 많은 노력을 하고 있습니다. 과거 높은 사망률을 가진 사스(SARS)나 에볼라(Ebola)와는 달리 COVID-19의 치사율은 오히려 비교적 낮은 편에 속합니다. 그럼에도 불구하고, 이렇게 오랜 기간 동안 우리를 괴롭히고 있는 근본적인 이유는 바로 COVID-19의 강력한 전염력 때문입니다.

감염자의 입, 호흡기로부터 나오는 비말, 침 등으로 인해 다른 사람에게 쉽게 전파가 될 수 있기 때문에 감염 확산 방지를 위해 무엇보다 중요한 것은 모든 사람이 마스크로 코와 입을 가려서 혹시 모를 감염자로부터의 전파 경로를 원천 차단하는 것입니다. 이를 위해 공공 장소에 있는 사람들은 반드시 마스크를 착용해야 할 필요가 있으며, 무엇 보다도 코와 입을 완전히 가릴 수 있도록 올바르게 착용하는 것이 중요합니다. 하지만 넓은 공공장소에서 모든 사람들의 올바른 마스크 착용 상태를 검사하기 위해서는 추가적인 인적자원이 필요할 것입니다.

따라서, 우리는 카메라로 비춰진 **사람 얼굴 이미지 만으로 이 사람이 마스크를 쓰고 있는지, 쓰지 않았는지, 정확히 쓴 것이 맞는지 자동으로 가려낼 수 있는 시스템**이 필요합니다. 이 시스템이 공공장소 입구에 갖춰져 있다면 적은 인적자원으로도 충분히 검사가 가능할 것입니다.

## Competition 관련 정보

-   대회 주최: [BoostCamp AI Tech](https://boostcamp.connect.or.kr/)
-   대회 진행 홈페이지: [AI Stages](https://stages.ai/)
## 🔍Project Overview

COVID-19의 확산으로 우리나라를 포함한 전 세계 사람들은 경제적, 생산적 활동에 많은 제약을 가지게
되었습니다. COVID-19 확산을 방지하기 위해서는 모든 사람이 올바르게 마스크를 착용하여 전파 경로를
원천 차단해야 합니다. 하지만, 이를 확인하기 위해서는 많은 인적자원이 소모되므로, 올바른 마스크 착용
여부를 자동으로 검출해주는 시스템이 필요합니다

## 🗂️Dataset
- Total : 4500

- 학습 데이터와 평가 데이터전체를 구분하기 위해 임의로 섞어서 분할하였습니다. 
- 학습 데이터셋이 아닌 나머지 40%의 데이터셋 중에서 20%는 public 테스트셋, 그리고 20%는 private 테스트셋으로 사용됩니다.
- Train : 2700
- Test : 1800 (900(public) + 900(private))
  
- 한 사람당 사진의 개수: 7 [마스크 착용 5장, 이상하게 착용(코스크, 턱스크) 1장, 미착용 1장]
- 이미지 크기: (384, 512)

![image](https://user-images.githubusercontent.com/59071505/168463193-5399fae7-5d19-4418-b95a-0dad912ee279.png)

## 🏆Result
- Rank : 7등 / 20팀
- Public_f1 : 0.7521
- Private_f1 : 81.2540

<img width="1085" alt="스크린샷 2022-11-11 오후 1 25 36" src="https://user-images.githubusercontent.com/69153087/201263035-fc44a69f-c35b-4248-8c93-777bfffb1d1f.png">

## Project Overview
+ 코로나 확산에 따른 일상생활에서 마스크 착용이 의무화가 되면서 감염을 막기위해서는 코, 입을 올바르게 착용하는 것이 중요한 상황
+ 공공장소에서 이를 검사하려면 추가적인 인적자원이 필요
+ 카메라에 비춰진 얼굴 이미지로 마스크 착용여부와 올바르게 쓴게 맞는지 가려내는 시스템이 필요  

## Objective
성별, 연령, 마스크 착용 여부에 따라 사진을 총 18개의 클래스로 분류

## How to Solve

EDA를 통해 데이터를 분석하고 분석한 결과를 바탕으로 데이터 전처리를 진행했다. 그 후 적절한 모델을 선정하여 학습시키고 다양한 기법들을 활용하여 성능을 증가시켜나갔다.  
자세한 내용은 Wrap up Report에 기술해 두었다.

## Data Overview
|class|mask|gender|age|
|---|---|---|---|
|0|Wear|Male|<30|
|1|Wear|Male|>=30 and <60|
|2|Wear|Male|>=60|
|3|Wear|Female|<30|
|4|Wear|Female|>=30 and <60|
|5|Wear|Female|>=60|
|6|Incorrect|Male|<30|
|7|Incorrect|Male|>=30 and <60|
|8|Incorrect|Male|>=60|
|9|Incorrect|Female|<30|
|10|Incorrect|Female|>=30 and <60|
|11|Incorrect|Female|>=60|
|12|Not Wear|Male|<30|
|13|Not Wear|Male|>=30 and <60|
|14|Not Wear|Male|>=60|
|15|Not Wear|Female|<30|
|16|Not Wear|Female|>=30 and <60|
|17|Not Wear|Female|>=60|  


## Explanation
+ **Best directory**  
학습된 모델을 모아놓은 directory

>모델 설명  

| 모델 이름 | 설명 |
| :--------: | :-------- |
| CoAtNet_81.pth | **CoAtNet-b0** transformation4. imbalancedsampler. label에 따라 다른 augmentation. label smoothing. |
| mask_model.pt | **EfficientNet-b0** transformation4. imbalancedsampler. label smoothing. Focal Loss. <57 label change |
| Resnet_80.pth | **ResNet18** transformation4. labelsmoothing. imbalancedsampler. label에 따른 augmentation. <58 label change |
| Resnet_mixup.pth | **ResNet18** transformation4. imbalancedsampling. Mixup. |


## 활용 기법

### EDA

- pandas,matplotlib,seaborn등의 라이브러리를 활용했다.
- 나이,성별 : Seaborn의 CountPlot 활용했다.
- 마스크 착용 여부 : Seaborn의 BarPlot 활용했다.

+ **EDA, Augmentation, Sampler.ipynb**  
EDA, Augmentation 기법 적용, Sampler 분석 노트북


### Augmentation
- ToGray: 흑백 효과를 추가하여 머리색이 나이를 판단하는 기준에 머리색뿐이 아닌 주름살같은 피부요인도 고려해보게끔 유도하였다.
- CourseDropOut: 사진에 임의의 hole을 발생시켜서 학습효과 향상을 기대하였다.
- ChannelDropOut: 임의의 색 변화를 통해 다양한 요인에서 학습을 시켰다.
- MultiplicativeNoise: Noise 효과를 줘서 화질이 조금 안좋은 사진에서도 학습시켰다.
- HorizontalFlip: 거꾸로 된 사람은 없기 때문에 좌우 반전만 시도했다.
- CenterCrop: 사람의 안면 부분만 따로 빼내기 위해 사용했다.
- Resize: 모델의 크기에 맞게 조정하기 위해 사용했다.
- Normalize: 사진의 색을 최대한 원본색에 가깝게 하기위해 사용했다.

### Class Imbalance & Data Labeling
- ImbalancedSampler 기법을 사용하여 under sampling과 over sampling을 적절히 섞었다.
- Smooth labeling 기법을 사용하여 one-hot encoding을 방지했다.
- Cross Entropy대신 Focal Loss를 활용했다.
- 60세 이상의 자료가 부족했기 때문에 57세 이상부터 60대로 분류했다.

+ **Preprocessing.ipynb**  
Data Pipeline 용 코드


+ **Ensemble.ipynb**  
Best directory에 있는 학습된 모델들을 soft-voting을 통해 valid 및 submission file을 만들 수 있는  코드
