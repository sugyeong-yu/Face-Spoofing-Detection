# Face-Spoofing-Detection
:books:**Our paper using this**
- Kim, So-Eui, Su-Gyeong Yu, and Eui Chul Lee. "Face spoofing detection using DenseNet." Proceedings of the Korea Information Processing Society Conference. Korea Information Processing Society, 2020.  
- Yu, Su-Gyeong, So Eui Kim, Kun Ha Suh, and Eui Chul Lee. "Face Spoofing Detection Using DenseNet." International Conference on Intelligent Human Computer Interaction. Springer, Cham, 2020.

Deep-Learning Model을 이용하여 Face spoofing attack을 detect 한다.
## Dataset
1. PR-FSAD
    - 3가지 각도(Bottom, Middle, Top) / 3가지 거리(Near, Middle, Distant)
    - 다양한 조명, 환경
    - 2가지 공격유형(print, replay)
2. CASIA-FASD
3. Replay-Attack

## Model
1. ResNet-18
2. DenseNet-121

## Result

<table>
  <tr>
    <td rowspan="2", colspan="2">Protocol</td>
    <td colspan="3">ResNet18</td>
    <td colspan="3">DenseNet121</td>  
  </tr>
  <tr>
    <td colspan="1">Precision</td>
    <td>Recall</td>
    <td>Acc</td>  
    <td colspan="1">Precision</td>
    <td>Recall</td>
    <td>Acc</td>  
  </tr>
  <tr>
      <td rowspan="3"> Protocol1</td>
      <td>Top</td>
      <td>94.92%</td>
      <td>97.39%</td>
      <td>97.39%</td>
      <td>96.01%</td>
      <td>97.96%</td>
      <td>97.96%</td>
    </tr>
      <tr>
      <td>Middle</td>
      <td>90.52%</td>
      <td>95.03%</td>
      <td>95.03%</td>
      <td>93.25%</td>
      <td>96.51%</td>
      <td>96.51%</td>
    </tr>
      <tr>
      <td>Bottom</td>
      <td>93.85%</td>
      <td>96.79%</td>
      <td>96.82%</td>
      <td>93.31%</td>
      <td>96.54%</td>
      <td>96.54%</td>
    </tr>
    
  <tr>
      <td rowspan="2"> Protocol2</td>
      <td>Near</td>
      <td>93.49%</td>
      <td>96.63%</td>
      <td>96.63%</td>
      <td>95.04%</td>
      <td>97.44%</td>
      <td>97.45%</td>
    </tr>
      <tr>
      <td>Distance</td>
      <td>91.63%</td>
      <td>95.61%</td>
      <td>95.62%</td>
      <td>92.13%</td>
      <td>95.93%</td>
      <td>95.91%</td>
    </tr>
      
   <tr>
      <td> Protocol3</td>
      <td>Total</td>
      <td>92.81%</td>
      <td>96.26%</td>
      <td>96.27%</td>
      <td>97.66%</td>
      <td>95.43%</td>
      <td>97.66%</td>
    </tr>
      <tr>
      <td rowspan="2"> Protocol4</td>
      <td>CASIA-FASD</td>
      <td>90.30%</td>
      <td>96.66%</td>
      <td>96.62%</td>
      <td>93.16%</td>
      <td>97.65%</td>
      <td>97.65%</td>
    </tr>
      <tr>
      <td>Replay-Attack</td>
      <td>99.69%</td>
      <td>99.90%</td>
      <td>99.90%</td>
      <td>99.90%</td>
      <td>99.97%</td>
      <td>99.97%</td>
    </tr>
</table>


|other Model|Precision|Recall|ACC|
|---|---|---|---|
|Resnet50|90.15%|94.82%%|94.82%|
|Resnet101|88.59%|93.95%|93.95%|
|Densenet169|93.61%|96.73%|96.73%|

- resnet18 : batch16, lr0.001
- resnet50 : batch8, lr0.001
- resnet101 : batch8, lr0.001
- Densenet121 : batch8, lr0.001 (replay : batch16, lr0.01)
- Densenet169 : batch16, lr0.001
