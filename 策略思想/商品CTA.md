# 商品CTA策略

**也可叫管理期货**

**股票量化接口限制 ,2016年新宠 **

**技术分析是最主要的**

- 技术指标作为过滤器
- 自己定义出场入场信号
- 加上加仓,减仓,资金管理的方法
- 构成CTA完整交易系统

**SR : 0.8-1就不错了, 因为本身波动就很大**

<img src="商品CTA.assets/image-20200301100057734.png" alt="image-20200301100057734" style="zoom:67%;" />



- 在CTA上的策略不一定适用于股票
- 投资于各类衍生品



## 市场规模

<img src="商品CTA.assets/image-20200301100519328.png" alt="image-20200301100519328" style="zoom:67%;" />



![image-20200301101151351](商品CTA.assets/image-20200301101151351.png)



## 商品品种

<img src="商品CTA.assets/image-20200301101641949.png" alt="image-20200301101641949" style="zoom:67%;" />![image-20200301101719395](商品CTA.assets/image-20200301101719395.png)

![image-20200301101719395](商品CTA.assets/image-20200301101719395.png)



## 交易规则

<img src="商品CTA.assets/image-20200301101758946.png" alt="image-20200301101758946" style="zoom:67%;" />



## 商品之间相关性

![image-20200301101950953](商品CTA.assets/image-20200301101950953.png)



- 螺纹钢和热卷相关性高达0.98
- 可以做pairtrading



## 趋势跟踪型

<img src="商品CTA.assets/image-20200301102234704.png" alt="image-20200301102234704" style="zoom:67%;" />

- 相互协同关系
- 波动大 ,夏普比率低



### 菲阿里四价策略

- 日内交易
- 四价 : 昨高 , 昨低 , 昨收 , 今开

<img src="商品CTA.assets/image-20200301104033244.png" alt="image-20200301104033244" style="zoom: 67%;" />

<img src="商品CTA.assets/image-20200301104331102.png" alt="image-20200301104331102" style="zoom:67%;" />


- 假突破问题
- 加过滤条件![image-20200301104627802](商品CTA.assets/image-20200301104627802.png)



### 修正TD模型

#### 买入信号

<img src="商品CTA.assets/image-20200301105006602.png" alt="image-20200301105006602" style="zoom:67%;" />

<img src="商品CTA.assets/image-20200301105908489.png" alt="image-20200301105908489" style="zoom:67%;" />



- 连跌6天
- 空方力量耗尽
- 四次计数 :多方能量积聚



#### 卖出信号

<img src="商品CTA.assets/image-20200301110406274.png" alt="image-20200301110406274" style="zoom:67%;" />

<img src="商品CTA.assets/image-20200301110113527.png" alt="image-20200301110113527" style="zoom:67%;" />



### Dual Thrust策略

<img src="商品CTA.assets/image-20200301111313032.png" alt="image-20200301111313032" style="zoom:67%;" />



**关键 : 上下轨的确定**

<img src="商品CTA.assets/image-20200301111427727.png" alt="image-20200301111427727" style="zoom:67%;" />



- k1 , k2 可以自己调整
- 认为市场上涨概率大 , 可以把 k1 调小

<img src="商品CTA.assets/image-20200301111511078.png" alt="image-20200301111511078" style="zoom:67%;" />

### ==ATR策略==

**可以跟海龟交易法结合使用**

**作为动态止盈止损的依据**

**这个指标和VIX很像 , 极小值蕴含危机**



<img src="商品CTA.assets/image-20200301112230512.png" alt="image-20200301112230512" style="zoom:67%;" />

**真实: 三个波幅里面最大的那个才是真实的波幅 ,==考虑跳空 : 第二个跳空高开 , 第三个跳空低开==**

<img src="商品CTA.assets/image-20200301113350689.png" alt="image-20200301113350689" style="zoom: 50%;" />

**极端值**

<img src="商品CTA.assets/image-20200301113301749.png" alt="image-20200301113301749" style="zoom:67%;" />



**策略:**
<img src="商品CTA.assets/image-20200301113811469.png" alt="image-20200301113811469" style="zoom:67%;" />



**止盈止损:**

<img src="商品CTA.assets/image-20200301114749802.png" alt="image-20200301114749802" style="zoom:50%;" />



**新的思路:**

- 挑选一些股票前期波动很小的
- 成交量很低的 , **地量地价**
- 某一天成交量急剧放大或者ATR突然上涨 , 资金注入

<img src="商品CTA.assets/image-20200301114219951.png" alt="image-20200301114219951" style="zoom: 50%;" />



### R-Breaker策略

- 日内策略
- 趋势加反转

<img src="商品CTA.assets/image-20200301120200905.png" alt="image-20200301120200905" style="zoom: 67%;" />

#### 交易原理

<img src="商品CTA.assets/image-20200301120703065.png" alt="image-20200301120703065" style="zoom:67%;" />

#### 价格计算

<img src="商品CTA.assets/image-20200301120325196.png" alt="image-20200301120325196" style="zoom:67%;" />

#### 触发条件

<img src="商品CTA.assets/image-20200301120805831.png" alt="image-20200301120805831" style="zoom:67%;" />



### 长线系统Aberration

- 可用于股票

- 每年交易次数不多
- 但是能把握住大机会

<img src="商品CTA.assets/image-20200301121254229.png" alt="image-20200301121254229" style="zoom:67%;" />





## 套利型

![image-20200301102949802](商品CTA.assets/image-20200301102949802.png)



- 相互竞争关系,你赚钱别人就赚不了
- 优势:
  - 风险小
  - 回撤小
- 问题:
  - 首先要有套利机会