# gin-Demo
Demo for run gin-framework


Demo-Framework base to : https://github.com/gin-gonic/gin
And others. 
Thanks for...

示例主体框架使用gin-framework,第三方包在demopacket完整打包,解压后可使用.
ps:直接解压demopacket包按结构存放即可.使用的都是开源包(后续列出来)

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