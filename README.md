## 前后端分离项目

包含基本的登录、注册、密码重置等功能，可以二次开发编写具体场景下的功能。
* 登录功能（支持用户名、邮箱登录）
* 注册用户（通过邮箱注册）
* 重置密码（通过邮箱重置密码）

登录功能：
* 用户登录成功后，才能访问index路径下的页面
* 用户如果没有登录，才会自动跳转到登录界面
* 如果一个用户请求不存在，则强制回到登录界面，如果已经登录，则回到index页面

登录解决方案：
* 无论是否已经登录，浏览器直接向后端请求用户信息
* 如果请求成功，说明已经登录
* 如果失败，说明没有登录，跳转到登录界面