# linxu上的一些安装
# jdk的安装

1.向centos服务器上传文件,可直接在centos上执行命令yum -y install lrzsz 程序会自动安装好,如果下载sz,上传使用rz.
2.把上传后的jdk包解压,使用tar -zxvf 
3.配置JavaHome,进入配置文件命令:vim/etc/profile,在底部添加
    #set java environment
    JAVA_HOME=/usr/local/src/java/jdk1.8.0_151
    CLASSPATH=.:$JAVA_HOME/lib.tools.jar
    PATH=$JAVA_HOME/bin:$PATH
    export JAVA_HOME CLASSPATH PATH
4.配置完成后,使用java -version来检查是否配置成功
