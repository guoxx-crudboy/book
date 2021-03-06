# activeJava8

## 1 为什么要关心java8

1.1 java怎么还在变

+ java在编程语言生态系统中的位置
+ 流处理
+ 用行为参数化吧代码传递给方法
+ 并行与共享的可变数据
+  java需要演变

1.2 java中的函数

+ 方法和Lambda作为一等公民
+ 传递代码：一个例子
+ 从传递方法到Lambda

1.3 流

1.4 默认方法

1.5 来自函数会变成的其他好思想

## 2 通过行为参数化传递代码

2.1 应对不断变化的需求

+ 初试牛刀：筛选绿苹果
+ 再展身手：把颜色作为参数
+ 第三次尝试：对你能想到的每个属性做筛选

2.2 行为参数化

2.3 对付啰嗦

+ 匿名类
+  第五次尝试：使用匿名类
+ 第六次尝试：使用Lambda表达式
+ 第七次尝试：将List类型抽象化

2. 4真是的例子

+ 用Comparator来排序
+ 用Runnable执行代码块
+ GUI事件处理

## 3 Lambda表达式

3.1 Lambda初识

3.2 在哪里以及如何使用Lambda

+ 函数式接口
+ 函数描述符

3.3 把Lambda付诸实践：环绕执行模式

+ 第一步：记得行为参数化
+ 第二步：记得函数式接口来传递行为
+ 第三步：执行一个行为
+ 第四步：传递Lambda

3.4 使用函数式接口

+ Predicate
+ Consumer
+ Function

3.5 类型检查、类型推断以及限制

+ 类型检查
+ 永远的Lambda，不同的函数式接口
+ 类型推断
+ 使用局部变量

3.6 方法引用

+ 方法引用初识
+ 构造函数引用

3.7 Lambda和方法引用实战

+ 第一步：传递代码
+ 第二步：使用匿名类
+ 第三步：使用Lambda表达式
+ 第四步：使用方法引用

3.8 复合Lambda表达式的有用方法

+ 比较器复合
+ 谓词复合
+ 函数复合

3.9 数学中的类似思想

+ 积分
+ 与java8的Lambda联系起来

## 4 引入流

4.1 流是什么

4.2 流简介

4.3 流与集合

+ 只能遍历一次
+ 外部迭代与内部迭代

4.4 流操作

+ 中间操作
+ 终端操作
+ 使用流

## 5 使用流

5.1 筛选和切片

+ 用谓词筛选
+ 筛选各异的元素
+ 截短流
+ 跳过元素

5.2 映射

+ 对流中每一个元素应用函数
+ 流的扁平化

5.3 查找和匹配

+ 检查谓词是否至少匹配一个元素
+ 检查谓词是否匹配所有元素
+ 查找元素
+ 查找第一个元素

5.4 归约

+ 元素求和
+ 最大值和最小值

5.5 付诸实践

+ 领域：交易员和交易
+ 解答

5.6 数值流

+ 原始类型流特化
+ 数值范围
+ 数值流应用：勾股数

5.7 构建流

+ 由值创建流
+ 由数组创建流
+ 由文件生成流
+ 由函数生成流：创建无限流

## 6 用流收集数据

6.1 收集器简介

+ 收集器用作高级归约
+ 预定义收集器

6.2 归约和汇总

+ 查找流中的最大值和最小值
+ 汇总
+ 连接字符串
+ 广义的归约汇总

6.3 分组

+ 分级分组
+ 按子组收集数据

6.4 分区

+ 分区的优势
+ 将数字按质数和非质数分区

6.5 收集器接口

+ 理解Collector接口声明的方法
+ 全部融合到一起

6.6 开发自己的收集器以获得更好的性能

+ 仅用质数做除数
+ 比较收集器的性能

## 7 并行数据处理与性能

7.1 并行流

+ 将顺序流转换为并行流
+ 测量流性能
+ 正确使用并行流
+ 高效使用并行流

7.2 分支/合并框架

+ 使用RecursiveTask
+ 使用分支/合并框架的最佳做法
+ 工作窃取

7.3 Spliterator

+ 拆分过程
+ 实现你自己的Spliterator

## 8 重构、测试和调试

8.1 为改善可读性和灵活性重构代码

+ 改善代码的可读性
+ 从匿名类到Lambda表达式的转换
+ 从Lambda表达式到方法引用的转换
+ 从命令式的数据处理切换到Stream
+ 增加代码的灵活性

8.2 使用Lambda重构面向对象的设计模式

+ 策略模式
+ 模板方法
+ 观察者模式
+ 责任链模式
+ 工厂模式

8.3 测试Lambda表达式

+ 测试课件Lambda函数的行为
+ 测试使用Lambda的方法的行为
+ 将复杂的Lambda表达式分到不同的方法
+ 高阶函数的测试

8.4 调试

+ 查看栈跟踪
+ 使用日志调试

## 9 默认方法

9.1 不断演进的API

+ 初始版本的API
+ 第二版API

9.2 概述默认方法

9.3 默认方法的使用模式

+ 可选方法
+ 行为的多继承

9..4 解决冲突的规则

+ 解决问题的三条规则
+ 选择提供了最具体实现的默认方法的几口
+ 冲突及如何显式的消除歧义
+ 菱形继承问题

## 10 用OPtional取代null

10.1 如何为缺失的值建模

+ 采用防御式检查减少NullPointerException
+ null带来的种种问题
+ 其他语言中null的替代品

10.2 Optional类入门

10.3 应用Optional的几种模式

+ 创建Optional对象
+ 使用map从Optional对象中提取和转换值
+ 使用flatMap链接Optional对象
+ 默认行为及解引用Optional对象
+ 两个Optional对象的组合
+ 使用filter剔除特定的值

10.4 使用Optional的实战示例

+ 用Optional封装可能为null的值
+ 异常与Optional的对比
+ 把所有内容整合起来

## 11 CompletableFutrue：组合式异步编程

11.1 Future接口

+ Future接口的局限性
+ 使用CompletableFutrue构建异步应用

11.2 实现异步API

+ 将同步方法转换为异步方法
+ 错误处理

11.3 让你的代码免受阻塞之苦

+ 使用并行流对请求进行并行操作
+ 使用CompletableFutrue发起异步请求
+ 寻找更好的方案
+ 使用定制的执行器

11.4 对多个异步任务进行流水线操作

+ 实现折扣服务
+ 使用Discount服务
+ 构建同步和有操作
+ 将两个CompletableFutrue对象整合起来，无论他们是否存在依赖
+ 对Future和CompletableFutrue的回顾

11.5 响应CompletableFutrue的completion事件

+ 对最佳价格查询器应用的优化
+ 付诸实践

## 12 新的日期和时间API

12.1 LocalDate、LocalTime、Instant、Duration以及Period

+ 使用LocalDate和LocalTime
+ 合并时间和日期
+ 机器的日期和时间格式
+ 定义Duration或Period

12.2 操作、解析和格式化日期

+ 使用TemporalAdjuster
+ 打印输出及解析日期-时间对象

12.3 处理不同的时区和历法

+ 使用和UTC的固定偏差计算时区
+ 使用别的日历系统

## 13 函数式的思考

13.1 实现和维护系统

+ 共享的可变数据
+ 声明式编程
+ 为什么要采用函数式编程

13.2 什么是函数式编程

+ 函数式java编程
+ 引用透明性
+ 面向对象的编程和函数式编程的对比
+ 函数式编程实战

13.3 递归和迭代

## 14 函数式编程的技巧

14.1 无处不在的函数

+ 高阶函数
+ 科里化

14.2 持久化数据结构

+ 破坏式更新和函数式更新的比较
+ 另一个使用Tree的例子
+ 采用函数式的方法

14.3 Stream的延迟计算

+ 自定义的Stream
+ 创建你自己的延迟列表

14.4 模式匹配

+ 访问者设计模式
+ 用模式匹配力挽狂澜

14.5 杂项

+ 缓存或记忆表
+ “返回同样的对象”意味着什么
+ 接合器

## 15 面向对象和函数式编程的混合：java8和Scala的比较

15.1 Scala简介

+ 你好啤酒
+ 基础数据结构：List、Set、Map、Tuple、Steam以及Option

15.2 函数

+ Scala中的一等函数
+ 匿名函数和闭包
+ 科里化

15.3 类和trait

+ 更加简介的Scala类
+ Scala的trait与java8的接口对比

## 16 几轮以及java的未来

16.1 回顾java8的语言特性

+ 行为参数化（Lambda以及方法引用）
+ 流
+ CompletableFutrue
+ Optional
+ 默认方法

16.2 java的未来

+ 集合
+ 类型系统的改进
+ 模式匹配
+ 更加丰富的泛型形式
+ 对不变形的更深层支持
+ 值类型

16.3 写在最后的话