# 接口：getStudentsS  [返回](../README.md)
用例： [学生列表](../用例/学生列表.md)

* 权限：
    学生/访客：不能看到WEB_SUM
    老师：可以看到WEB_SUM。

* 功能：
    返回所有学生的列表。

* API请求地址：
   接口基本地址/com/api/getStudentsS

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
                         "UPDATE_DATE": "2018-06-01 19:24:41"},
                       },
                       {
                       ....其他学生
                       }  
                },
               "msg": "操作成功"
            }

* 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |code|请求响应状态|
  |total|返回学生人数|
  |data|所有学生的信息数组|
  |GITHUB_USERNAME|GITHUB 用户名|
  |STUDENT_ID|学号|
  |CLASS|班级|
  |NAME|真实姓名|
  |UPDATE_DATE|GitHUB用户名修改日期|