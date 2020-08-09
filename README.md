学生信息管理系统
======


1.题目说明
------
本项目是使用Jsp+Sevlet+JavaBean实现的学生体质信息管理系统，样式使用了LayUI前端框架


2.需求描述
------
  为实现学校对学生体质基本信息的管理，方便学校对学生信息的查插删改
  ![image](https://github.com/wys9853/Student-Information-Management-System/blob/master/%E5%9B%BE%E7%89%871.png)





3.功能描述
-------
（1）通过左侧导航栏实现五种不同的功能

（2）实现了添加学生信息：学号，姓名，性别，年龄，身高，体重，这六条数据的插入

（3）实现了通过学生学号删除学生信息的功能

（4）通过学生学号单独查询学生信息

（5）列出数据库中全部学生信息

（6）修改学生信息包括 学号，姓名，性别，年龄，身高，体重

（7）使用了layUI前端框架对图标，按钮，页面转场进行了美化处理





4.设计思路
-----
（1）Jsp+Sevlet+JavaBean
JSP负责与用户的人机交互，Servlet负责流程控制，JavaBean负责数据操作。
可以理解为JSP充当视图，Servlet充当控制器，JavaBeans充当模型


（2）
1.View层（JSP）,前台交互,比如我们注册时的数据等等,serlvet就是与前台数据进行交互的
2.Contrller层（servlet充当）：Model与View之间沟通的桥梁， 这个层有业务处理,用户的注册登录就可以看做是User的业务,我们就需要将相关的处理代码写到这个层中。
3.Model层：实现系统的业务逻辑，即javaBean，常见的就是封装对象的属性、数据库连接操作等。

（3）
1.M层：创建com.dao和bean包用于持久化，如数据库连接，sql语言
2.V层：jsp文件用于前端交互，网页显示数据，用户操作
3.C层：servlet对业务功能进行处理查插删改

![image](https://github.com/wys9853/Student-Information-Management-System/blob/master/%E5%9B%BE%E7%89%872.png)
