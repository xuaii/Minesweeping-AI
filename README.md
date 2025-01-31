<<<<<<< HEAD
### 1. AI 方法

划分连通块 + 解线性方程组 + 枚举变元 + 随机点

[扫雷AI](https://gitee.com/xuaii/boom/blob/master/ai/AI.md)

运行结果：

![None](https://gitee.com/xuaii/boom/raw/9a4ec33191778a5ead3bd408b672c404e4a0ba38/result/impicture_20210421_030325.png "None")

### 2. 运行方式

自动扫雷：

```shell
python aitest.py ai
```

手动扫雷：

```shell
python aitest.py manual
```

### 3. 文件结构

* game
  * app                  一个CGame 类， 提供游戏接口
  * cmdins      	  各个命令的实现
    * check       点击一个单元格 1 [x] [y]
    * debug      用于调试（偷看） 2：显示所有雷， 3隐藏所有雷
    * flag           用于标记雷 4 [x] [y]
  * command      命令管理器
  * defines           定义常量
  * grids               网格类
  * unit                 单元格类
  * utils                工具函数
* ai
  * ai.py                       实现 AI 的函数集
  * aitest.py                用于测试（人工和AI）
  * gauss.py			    解非齐次线性方程组 + 枚举自由变元 的函数集
  * AI.md                     实现思路说明
* 运行结果                截图和gif
* Enumerate            之前用 C++实现的枚举部分

