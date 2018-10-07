# 用construct2制作“勒布朗暴打杜兰特”小游戏

## 楔子：
2018年NBA新赛季已经正式开始，面对荆州勇士队抱团妄图塑造王朝的局面，看三旬老汉LBJ如何突破罗网，成就湖人总冠军。

## 玩法：
玩家通过键盘控制LBJ的移动避开杜兰特的围追堵截，并用鼠标控制发射篮球击败杜兰特。

## 人设与道具：
### 1.玩家：LBJ，著名NBA球星
### 2.敌人：杜兰特，LBJ的死敌
### 3.篮球：LBJ的武器，击中杜兰特可将他消灭

动态图![](images\5.gif)

## 游戏设计：
![](images\6.png)
![](images\7.png)
### Behavior
玩家：  8 direction movement
       Scroll To
       Bound to layout
篮球：Bullet movement
敌人：Bullet movement
      destroy ouside layout
爆炸特效:Fade
### Event
Add condition system>every tick
Add action player.Set angle towards position>X:Mouse.X
Y:Mouse.Y
Add condition bullet>Mouse >on click>left clicked
Add action player>spawn another object>for object,choose the bullet

## 体悟：
不足:怪物数量太少，游戏过于简单
体会：自己做一个游戏还是很有成就感的，以后会继续尝试。
