# 接口：changeScores  [返回](../README.md)
用例： [修改成绩](../用例/修改成绩.md)

* 权限：
    老师修改成绩必须登录

* 功能：
    根据选择的学期和课程，修改实验的成绩。

* API请求地址：
   接口基本地址/com/api/changeScores

* 请求方式 ：
   POST

* 请求参数说明:
    无

* 返回实例：
    
       {
               "code": 200, 
               "total": 62,              
               "data": {
                   {
                      "GITHUB_USERNAME": "zhangsan",
                       "STUDENT_ID": "201510414200",
                        "CLASS": "软件(本)15-2",
                        "NAME": "张三",
                      "evaluates":{
                         ...每个实验的评价项，
                         "AVERAGE":平均成绩
                     },
                      "TERM_NAME": "学期",
                       "COURSENAME": "课程名称",
                },
                {
                    ...其余学生信息
                },
               "msg": "操作成功"
            }

* 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |code|请求响应状态|
   |total|返回学生人数|
  |data|该学生的信息数组|
    |data|所有学生的信息数组|
    |GITHUB_USERNAME|GITHUB 用户名|
    |STUDENT_ID|学号|
    |CLASS|班级|
    |NAME|真实姓名|
  |evaluates|评价数组|
  |AVERAGE|每个学期每个课程的所有实验的平均成绩|
  |TERM_NAME|成绩所属的学期|
  |COURSENAME|成绩所属的课程名称|
 