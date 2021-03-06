# 实验一：业务流程建模
|  学号  |  班级  |  姓名  |  照片  |
|  :----    |  :----    |  :----   |  :----   |
|  201510414230|软件（本）15-2|朱鹃|无|

### 流程图1：考试及成绩管理流程

##### plantUML源码如下：

     |教务处|
     :安排考试;
     :考试安排表;
     |教师|
     :出卷;
     fork
     :A、B试卷;
     fork again
     :打印审批卷;
     |系主任|
     :审批签字;
     :打印审批表;
     end fork
     |教务处|
     :打印试卷;
     :试卷;
     |学生|
     :参加考试;
     :答卷;
     |教师|
     :阅卷出成绩;
     fork
     :答卷;
         :装订存档;
     fork again
     :成绩单;
     |教务处|
     if(有不及格吗？)then(有)
         :安排补考;
         :补考安排表;
         |教师|
          :'||';
     |教务处|
     else
         stop
     endif
     |教师|
     end fork
     :期末流程结束;
  
 ##### 业务流程图如下：
![图片](1.png)

##### 流程说明
这是一个期末考试的流程，该流程图依照主要业务绘制，
由上至下，由左至右，按照考试的步骤来，然后这些步骤分
布在不同的角色上。

### 流程图2：客户维修服务流程

##### plantUML源码如下：


    |客户|
    start
    :申请服务;
    |业务经理|
    if(是新客户吗？) then (是)
       :登记客户信息;
       else (不是)
       endif
       :上门勘察;
       :制定方案;
    |客户|
    if (满意吗？) then (否)
        stop
    else (是)
        :签订服务合同;
        |业务经理|
        fork
            :安排工人;
         fork again
             :安排材料;
        end fork
        :填写派工单;
        |工人|
           :领取材料;
           :上门服务;
         |客户|
            :验收并填写反馈意见;
          |业务经理|
              :交回派工单;
           |财务人员|
               :结算收款;
               stop

#### 业务流程图如下：
![图片](2.png)

##### 流程说明
这是一个客户维修服务流程，该流程图较上一个图进行了进一步的细化，
分工更加明确。