# 实验二： 用例建模

## 一、实验目标

- 1.使用MarkDown文件写报告
- 2.选题并用例建模

## 二、实验内容

- 1.选题
- 2.在StarUML中画建模用例图
- 3.在github中写实验报告

## 三、实验步骤

- 1.选题，在github上的lssue中提交给老师  
    #474 电脑配件信息管理系统  
    - 1.管理员添加电脑配件信息  
    - 2.用户查看电脑配件信息
- 2.画图
    - 添加一个参与者命名为管理员
    - 添加一个用例：添加电脑配件信息
    - 连接管理员和添加电脑配件信息
    - 添加一个参与者命名为用户
    - 添加一个用例：查看电脑配件信息
    - 连接用户和查看电脑配件信息

## 四、实验结果

![用例图](./Lab2_UseCaseDiagram1.jpg)  
图1：电脑配件信息管理系统的用例图

## 表1：添加电脑配件信息用例规约  

用例编号  | UC01 | 备注  
-|:-|-  
用例名称  | 添加电脑配件信息  |   
前置条件  |      | *可选*   
后置条件  | 管理员把电脑配件信息添加到系统     | *可选*   
基本流程  | 1. 管理员点击添加配件信息链接  |*用例执行成功的步骤*    
~| 2. 系统显示添加电脑配件信息页面  |   
~| 3. 管理员填写电脑配件的信息，点击添加按钮  |   
~| 4. 系统根据配件名称在内部检索，确认系统内部不存在该电脑配件信息，保存电脑配件信息  |   
~| 5. 系统提示添加成功 |  
扩展流程  | 4.1 系统检查发现电脑配件信息已存在，提示"系统已存在此电脑配件信息"   |*用例执行失败*    
~| 4.2 系统检查发现填写的数据与要求冲突，提示"用户输入的数据不合法"  |

## 表2：查看电脑配件信息用例规约  

用例编号  | UC02 | 备注  
-|:-|-  
用例名称  | 查看电脑配件信息  |   
前置条件  |      | *可选*   
后置条件  | 用户查看电脑配件信息     | *可选*   
基本流程  | 1. 用户点击查找配件信息链接  |*用例执行成功的步骤*    
~| 2. 系统显示查找电脑配件信息页面  |   
~| 3. 用户填写电脑配件名称，点击查找按钮  |   
~| 4. 系统检查名称不为空，查询电脑配件信息  |   
~| 5. 系统显示电脑配件信息 |  
扩展流程  | 4 系统检查发现名称为空，提示"电脑配件名称不能为空"  |*用例执行失败*    
