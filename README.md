# gin-Demo
Demo for run gin-framework


Demo-Framework base to : https://github.com/gin-gonic/gin
And others. 
Thanks for...

示例主体框架使用gin-framework,第三方包在demopacket完整打包,解压后可使用.
ps:直接解压demopacket包按结构存放即可.使用的都是开源包(后续列出来)


目录结构:
|gin-Demo<br> 
|---bin          #固定目录(不懂请查找资料)<br> 
|---pkg          #固定目录(不懂请查找资料)<br> 
|---demopacket   #第三方包(工具)，编译时go会自动选择<br> 
|---src          #固定目录(不懂请查找资料)<br> 
|------github.com   #包<br> 
|------gopkg.in     #包<br> 
|------demo         #主体应用<br> 
|----------config      #配置<br> 
|----------lang        #语言<br> 
|----------middleware  #中间件<br> 
|----------modules     #模块<br> 
|----------router      #正式路由<br> 
|----------services    #服务组件<br> 
|----------ticker      #定时器<br> 
|----------trouter     #调试路由<br> 
|----------utils       #工具包<br> 
-----------main.go     main<br> 

ps:有些写的仓促比如config.go,lang.go后期会整合进来<br> 
框架使用传统mvc的设计模式进行构建:控制,模型,业务,验证等已分离.具体请看modules。

数据库连接示例:
```go
    Handler := mysql.GetDefault()
```

使用redis:(redis不支持连接池)

```go
    redisHanlder := redis.GetRedisCache()
    redisHanlder.Set(tKey, _currToken, loginTime)
```
有些错误判断未处理，请保证配置正确具体看配置目录下test.ini或prod.ini

语言包使用
```go
    //api lang里
    lang.GetLangTip(c, "Index", "loginSuccess")
```


验证器:
这里验证器使用了可配置化处理,开发者可以轻松配置验证规则，无需繁琐封装,支持中英文切换,具体参阅代码.
基于thedevsaddam/govalidator进行上层封装!




