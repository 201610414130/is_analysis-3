# 接口：login  [返回](../README.md)
用例： [登录](../用例/登录.md)

* 权限：
    老师评定成绩必须登录

* 功能：
    根据选择的学期和课程，评定每个实验的成绩。

* API请求地址：
   接口基本地址/com/api/login

* 请求方式 ：
   POST

* 请求参数说明:
    无

* 返回实例：
    
       {
               "code": 200,                ,              
               "data": {
                 
                       "STUDENT_ID": "201510414200",
                        "PASSWORD":"*****",
                },              
               "msg": "操作成功"
            }

* 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |code|请求响应状态|
    |data|所有学生的信息数组|
    |STUDENT_ID|学号|
    |PASSWORD|密码|
   |msg|操作信息|
 