# gin-Demo
Demo for run gin-framework


Demo-Framework base to : https://github.com/gin-gonic/gin
And others. 
Thanks for...

示例主体框架使用gin-framework,第三方包在demopacket完整打包,解压后可使用.
ps:直接解压demopacket包按结构存放即可.使用的都是开源包(后续列出来)

|gin-Demo
|---bin          #固定目录(不懂请查找资料)
|---pkg          #固定目录(不懂请查找资料)
|---demopacket   #第三方包(工具)，编译时go会自动选择
|---src          #固定目录(不懂请查找资料)
|------github.com   #包
|------gopkg.in     #包
|------demo         #主体应用
|----------config      #配置
|----------lang        #语言
|----------middleware  #中间件
|----------modules     #模块
|----------router      #正式路由
|----------services    #服务组件
|----------ticker      #定时器
|----------trouter     #调试路由
|----------utils       #工具包
-----------main.go     main