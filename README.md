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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
      <tr>
      <td>Middle</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
        </tr>
      <tr>
      <td>Bottom</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
      <tr>
      <td> Protocol3</td>
      <td>Total</td>
      <td></td>
      <td></td>
      <td></td>
      <td>97.66%</td>
      <td>0.9543</td>
      <td>0.9766</td>
    </tr>
      <tr>
      <td rowspan="2"> Protocol4</td>
      <td>CASIA-FASD</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
      <tr>
      <td>Replay-Attack</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
</table>

