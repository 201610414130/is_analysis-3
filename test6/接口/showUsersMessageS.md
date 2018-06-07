# 接口：showUsersMessageS  [返回](../README.md)
用例： [查看用户信息](../用例/查看用户信息.md)

* 权限：
    学生查看信息必须登录

* 功能：
   显示用户的个人信息

* API请求地址：
   接口基本地址/com/api/showUsersMessageS

* 请求方式 ：
   POST

* 请求参数说明:
    无

* 返回实例：
    
       {
               "code": 200,                         
               "data": {
                   
                      "GITHUB_USERNAME": "zhangsan",
                       "STUDENT_ID": "201510414200",
                      "CLASS": "软件(本)15-2",
                       "NAME": "张三",                        
                    }
               "msg": "操作成功"
            }

* 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |code|请求响应状态|
  |data|该老师的信息数组|
    |GITHUB_USERNAME|GITHUB 用户名|
    |STUDENT_ID|学号|
    |NAME|真实姓名|
  |CLASS|班级|
  |msg|操作信息|
 
 