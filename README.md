# game-template
JavaScript h5 games

### game design
牌名：理财牌
发牌员：控制生成3连
卡牌类游戏：
2 3 4 5 | 6 7 8 9 |
J Q K A |  万能牌

Auto:计算
玩家1，玩家2，玩家3，玩家4
3局两胜制度，3个玩家的时候，进行轮空
3摞牌，
1. 摸牌阶段：可以选择使用宝藏牌
2. 摸牌阶段：可以出售棋子，1级3连棋子加钱（+3），2级3连棋子加血（+4/加钱+9），3级给加血/加血骰子（5-10）
3. 棋子购买 1级1金币，2级2金币，3级3金币，4级4金币， 个人理财金币上限为50金币。
4. 可以花2块钱进行刷新，每回合刷新次数不限
5. 出牌阶段：第1回合只能默认第一摞牌，后面回合任意选择
6. 出牌阶段：每摞限制五张牌，有数字挨着的合并为0，
7. 战斗阶段：对比3摞卡牌的大小，3摞2胜者赢，败者掉血：(胜者等级 + 2)  X 胜者胜利局数
8. 结束阶段：获取本金+回合金币+理财+连胜奖励（+1金币）+连败奖励（+1金币）
9. 所有战斗阶段完成之后才能进入下阶段的开始

回合时长：

回合数| 摸牌阶段| 战斗阶段| 结束阶段| 
1 | 5 | 计算时间| 计算时间|
2 | 10 | 计算时间| 计算时间
3 | 15 | 计算时间 | 计算时间
4 | 15 | 计算时间 | 计算时间
5 | 15 | 计算时间 | 计算时间
6 | 15 | 计算时间 | 计算时间
7 | 20 | 计算时间 | 计算时间
8 | 20 | 计算时间 | 计算时间
9 | 30 | 计算时间 | 计算时间
10 | 30 | 计算时间 | 计算时间
11 | 30 | 计算时间 | 计算时间
12 | 40 | 计算时间 | 计算时间
13 | 40 | 计算时间 | 计算时间



棋子出售的金币限制为1，2，3，4
卡牌数量
 (2, 3, 4, 5) X 8
 (6, 7, 8, 9) X 8
（J Q K A） X 6
万能牌 X 4张，用完一张之后就牌库重新生成4张

每人54点初始血量；
回合数设计，理财方案设计
获取骰子数量，奖励骰子数量，连胜奖励：金币骰子、血量骰子
金币骰子：连败奖励

鏖战模式：每回合玩家掉半血，1血的时候持续2回合死亡

宝藏牌设计：（每5个回合给一次选择机会）
1. 花光全部金币 英雄一回合无敌
2. 将血量减半，获得10枚金币（不计算当前回合的10金币理财）
3. 不做选择


游戏模式：(强制天梯)
1. 天梯模式 （每日4局3胜可以晋级， 层级保级）
等级设置：兵，士，象，马，炮，车，帅（色彩分类）
赢一场+星级

2. 竞技模式 入场券：12金 5-2模式（赢2场回本，3场奖励虚拟豆（0豆一金），4胜奖励10金，5连胜奖励20金）
赢一场+金币
每日竞技场连胜上限200金，过期之后，大于2胜只返还12金

3. 人机模式

4. 每日任务： 金币任务，成就任务，自动登录签到（不包括玩家连续签到）

5. 站内信：活动奖励领取通知
6. 每个人的收藏空间：理论上无限大，层级记录收藏

7. 卡顿解决方案： 轮播特色文字，小技巧