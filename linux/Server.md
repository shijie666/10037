# 就攒个服务器吧
> 休息的时候总想搞点事情，探索下新技术，这些探索总是需要一些配置，每次搞都要自己部署一遍，不如来个一步到位的。于是想要自己赞个服务器。

```text
服务器配置  
1. OS: linux版CentOS 8.2 x64   
2. JDK: jdk1.8.271
```
1. 服务器系统，我还是模拟生产上，选择CentOS  
> 我选虚拟机，当然你也可以选WSL，具体怎么安装操作的，推荐去看开源中国的教程。  

2. 安装JDK，下载好tar.gz包后，上传到CentOS中  
> 1)解压：tar zvxf xxx  
>   重命名目录: mv a b   将目录 a 重命名为 b  
> 2)配置参数  
>   vi /etc/profile  
>   export JAVA_HOME=/usr/local/jdk8  #上面的 JDK 解压地址  
    export CLASSPATH=.:$JAVA_HOME/jre/lib/rt.jar:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar  
    export PATH=$PATH:$JAVA_HOME/bin  
  
> 3)生效命令：source /etc/profile  
  4)测试命令：java -version  
>   

