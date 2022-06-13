.. ChapterFour documentation master file, created by
   sphinx-quickstart on Mon Jun 13 15:46:54 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Lab3:Persistence Ignorance
======================================
小组成员：
'''''''''
201931990526   楼吉诚
^^^^^^^^^^^^^
201931990524   李远帆
^^^^^^^^^^^^^
201931990523   李森特
^^^^^^^^^^^^^
201931990521   康净焮
^^^^^^^^^^^^^
201931990528   潘林鑫
^^^^^^^^^^^^^

Abstract
--------

 Understand the Repository Pattern.
 Understand the Service Layer Pattern.
 Understand why it is important to separate business logic from data storage techniques.

Introduction
------------

In our textbook, we use SQLAlchemy to implement the Repository Pattern by defining a class called
SQLAlchemyRepository in repository.py. This repository implementation depends on a SQLAlchemy
session object and the PostgreSQL database. In this lab, you are going to use a non-database strategy
while implementing the Repository Pattern. More specifically, you will define a repository class called
PickleRepository. As the class name indicates, this class will use a pickle file as the infrastructure. A
pickle file is simpler than a database, isn’t it?

Methods and materials
---------------------

①

Results
-------
演示视频链接：https://cloud.zjnu.edu.cn/share/e0ee5c5956faf49f4626d504b2


Table 1
~~~~~~~

+--------------------------------------+---------+-------------------+
| question                             | ColdDew | BeginningOfSpring |
+======================================+=========+===================+
| Lines of code in main.py (excluding  | 498     | 114               |
| blank lines)                         |         |                   |
+--------------------------------------+---------+-------------------+
| Number of HTML files in folder       | 2       | 9                 |
| templates                            |         |                   |
+--------------------------------------+---------+-------------------+
| Has a service layer? Answer Yes or   | No      | Yes               |
| No.                                  |         |                   |
+--------------------------------------+---------+-------------------+
| Front-end and back-end coupling.     | Weak    | Strong            |
| Answer Strong or Weak.               |         |                   |
+--------------------------------------+---------+-------------------+
| Number of module-level dependencies  | 9       | 21                |
+--------------------------------------+---------+-------------------+

ColdDew : 2 BeginningOfSpring : 4

BeginningOfSpring 更容易理解和维护。 理由： 1.
BeginningOfSpring版本将原本全部堆积在main.py中的大量功能性代码进行了分类，这样在未来如果某项功能出现错误，可以更快地定位错误发生的位置。
2.
BeginningOfSpring版本将原本混杂在main.py中的html代码移出到template中，使代码更加简洁。

End
~~~
