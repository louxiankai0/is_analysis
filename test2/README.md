# 实验2 图书管理系统用例建模
|    学号    |       班级       |      姓名     |    照片    | 
|:-------:|:------------- | ----------:|----------:|
|   201510414412  |     2015级4班    |   楼轩恺   |  |
## 1. 图书管理系统的用例关系图

### 1.1 用例图PlantUML源码如下：

``` usecase
@startuml
Left to right direction
:图书管理员: as 1
:读者: as 2
:系统管理员: as 3
rectangle 图书管理系统{
1-->(登录)
1-->(查询图书信息)
1-->(更改图书信息)
1-->(借阅管理)
1-->(读者管理)
2-->(登录)
2-->(查询图书信息)
2-->(预定图书)
2-->(借书)
2-->(还书)
(发布新公告) <-- 3
(管理图书管理员) <-- 3
(维护系统) <-- 3
(登录) <-- 3
(查询图书信息) <-- 3
(更改图书信息) <-- 3
(借阅管理) <-- 3
(读者管理) <-- 3

(登录)<.(找回密码):<extends>
(借书)<.(续借):<extends>
(还书)<.(缴纳罚金):<extends>
}

@enduml
```
###1.2.用例图如下
![usecase](图书管理系统的用例图.png)