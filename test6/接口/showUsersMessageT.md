# 接口：showUsersMessageT  [返回](../README.md)
用例： [查看用户信息](../用例/查看用户信息.md)

* 权限：
    老师查看信息必须登录

* 功能：
    显示用户个人信息

* API请求地址：
   接口基本地址/com/api/showUsersMessageT

* 请求方式 ：
   POST

* 请求参数说明:
    无

*    
       {
                 "code": 200,                         
                 "data": {
                     
                        "GITHUB_USERNAME": "zhangsan",
                         "TEACHER_ID": "201510414200",
                          "DEPARTMENT": "学工办",
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
      |TEACHER_ID|工号|
      |NAME|真实姓名|
    |DEPARTMENT|所属部门|
    |msg|操作信息|
   