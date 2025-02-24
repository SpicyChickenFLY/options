# 练习题

## 1.11 仔细解释卖出一个看涨期权同买入一个看跌期权之间的区别
当交易员认为股票未来会有下跌的可能，
* 可以选择卖出一个看涨期权
    其主要收益就是期权合约金，主要亏损则是股价上涨幅度超出了期权合约金的差值
    如果大跌，多头将不会行使期权，白赚期权合约金
    收益有限，损益无限
* 也可以选择买入一份看跌期权
    其主要亏损是期权合约金，主要盈利是股价的下跌幅度超出了期权合约金差值
    亏损有限，潜在收益大

## 1.12 一个投资者承约了一个远期合约的空头：在该合约中，投资者能够以1.3000的汇率（美元/英镑）卖出100,000英镑。当远期合约到期时汇率为（a)1.29或（b）1.32时，投资的损益分别为多少？
(a) (1.30000 - 1.29) * 100000 = 1000美元
(b) (1.30000 - 1.32) * 100000 = -2000美元

## 1.13 某交易员承约期货价格每磅 ㊟ 【1磅=453.592克。】 50美分的棉花远期合约的空头。合约的规模是50000磅棉花。当合约结束时棉花的价格分别为：(a)每磅48.20美分；(b)每磅51.30美分。对应以上价格交易员的损益为多少？
(a) (48.20 - 50) * 50000 = -90000美分
(b) (51.30 - 50) * 50000 = 65000美分

## 1.14 假定你承约了一个执行价格为40美元的看跌期权空头，期限为3个月，股票的当前价格为41美元，1份看跌期权合约的规模是100股股票。你做出的是什么承诺？你的损益将是什么？
我做出的承诺为在3个月后将以40美元每股的价格买入100股的股票
我的损益将是：
* 假设股价高于行权价，卖家将不会行权，我将收益期权金
* 假设股价为低于行权价，我将收益期权金-(行权价-股价)

## 1.15 假设你认为某股票价格将要上升，股票的当前价格为29美元，而3个月期限、执行价格为30美元的看涨期权价格为2.9美元，你总共有5800美元的资金。说明两种投资方式：一种是利用股票，另一种是利用期权。每种方式的潜在损益是什么？
两种投资的具体实施方式为：
1. 使用5800美元在即期市场购买了200股的股票
2. 使用5800美元购买了20份看涨期权

3个月后：
* 假设股价为36美元(大涨)
    1. 第一种方式将收益(36 - 29) * 200 = 1400美元
    2. 第二种方式将收益(36 - 30 - 2.9) * 100 * 20 = 6200美元

* 假设股价为33美元(小涨)
    1. 第一种方式将收益(33 - 29) * 200 = 800美元
    2. 第二种方式将收益(33 - 30 - 2.9) * 100 * 20 = 200美元

* 假设股价为25美元(小跌)
    1. 第一种方式将损失(25 - 29) * 200 = 800美元
    2. 第二种方式将损失5800美元

即：
1. 股票投资方式 - 潜在收益和亏损变动成正比，风险低
2. 期权投资 - 潜在收益高（杠杆效应），但亏损有限于期权金


## 1.16 假如你拥有5000股股票，每股价格为25美元。你如何采用看跌期权使你投资的价值在将来4个月内得到保护？
购买一份4个月期限的看跌期权，如果未来股票涨了，不行权；如果跌了，行权卖出股票

## 1.17 股票在最初发行时会给公司提供资金，对期权来讲这种说法是否正确？
不知道

**纠正**
股票发行：公司通过发行股票筹集资金
期权：期权是衍生品，不会为公司提供资金，只是投资者间的合约

## 1.18 解释为什么期货合约既可以用于投机也可以用于对冲。
投机是利用了期货的杠杆效应的原理，用过预测价格变动赚取利润
对冲是利用了期货对未来的价格的不确定性设置一个保障(锁定未来价格)

## 1.19 假如一份在3月到期的看涨期权的价格为2.5美元，期权执行价格为50美元。假设期权一直被持有至到期日，在什么情形下期权持有人会盈利？在什么情形下持有人会行使期权？画出期权多头的盈利与在期权到期时股票价格之间关系的图形。
当3月份股价高于52.5美元时持有人会盈利；
当3月份股价高于50美元时持有人会行权；
设到期日股价为x美元时持有一份看涨期权多头盈利为y美元，关系函数为：
y = {
    -2.5 , x <= 50
    x - (50 + 2.5), x > 50
}

## 1.20 假如一个在6月到期、执行价格为60美元的看跌期权价格为4美元。假设期权被一直持有至到期日。在什么情形下期权的卖出方会盈利？在什么情形下期权会被行使？画出一个期权空头在到期时的收益与股票价格之间的关系图。
当6月份股价高于56美元时期权空头会盈利；
当6月份股价高于60美元时期权多头会行权；
设到期日股价为x美元时持有一份看涨期权多头盈利为y美元，关系函数为：
y = {
    x - (60 - 4), x <= 60
    4 , x > 60
}

## 1.21 现在是5月，一位交易员卖出了一份9月到期的看涨期权，其执行价格为20美元。当前的股票价格为18美元，期权价格为2美元。如果期权一直被持有至9月，那时股票价格为25美元，讨论投资者的现金流状况。
交易员卖出期权时收益2美元/每股期权金
到期股价为25美元，买方行权，交易员盈利(2 - (20 - 5)) = -3 美元/每股
