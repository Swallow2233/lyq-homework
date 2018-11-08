# HTML5游戏设计与制作

## 游戏策划

1.故事背景<br/>
一天，伐木工小林结束了一天的工作，决定在森林里休息。当他醒来，他惊讶地发现发现自己躺在一堆金币上。但这时，一阵狂风吹过，小林急忙躲到一旁的树丛中。当狂风过去，他发现金币堆已经被吹跑了，地上只剩一枚金币，于是，他决定深入森林去寻找金币......<br/>
![](images/lab08/Comic_01.png)<br/>
![](images/lab08/Comic_02.png)<br/>

2.玩法<br/>
通过键盘上的方向键控制小林，找到金币堆即为游戏结束，若不慎掉落则会重新开始游戏。<br/>

3.人设和物品<br/>
伐木工小林：对重复的工作感到厌烦，总希望能够一夜暴富。<br/>
金币堆：小林一直追求的财富，具有极高的价值，只是，它是真的吗......<br/>

## 游戏设计

Object Name:Player<br/>
Attributes:<br/>
![](images/lab08/Player1.png)<br/>
(480,1538)<br/>
Collaborator:Gold<br/>
Events & Actions:左右移动，向上跳跃<br/>

Object Name:Gold<br/>
Attributes:<br/>
![](images/lab08/Endgold.png)<br/>
(3827, 1217)<br/>
Collaborator:Player<br/>
Events & Actions:触发游戏结束<br/>

Object Name:Stone<br/>
Attributes:<br/>
![](images/lab08/Stein.png)<br/>
Collaborator:None<br/>
Events & Actions:固定不动<br/>

Object Name:Stone2<br/>
Attributes:<br/>
![](images/lab08/Stone.png)<br/>
Collaborator:None<br/>
Events & Actions:固定不动<br/>

Object Name:Stone3<br/>
Attributes:<br/>
![](images/lab08/Stone_1_2.png)<br/>
Collaborator:Player<br/>
Events & Actions:固定不动, Player向下时可穿过<br/>

## 游戏实际效果

![](images/lab08/game1.gif)<br/>

![](images/lab08/game2.gif)<br/>

![](images/lab08/game3.gif)<br/>