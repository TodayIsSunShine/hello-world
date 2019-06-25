# linxu上的一些安装
# jdk的安装

1.向centos服务器上传文件,可直接在centos上执行命令yum -y install lrzsz 程序会自动安装好,如果下载sz,上传使用rz.
2.把上传后的jdk包解压,使用tar -zxvf 
3.安装jdk
 yum -y install java-1.8.0-openjdk*

export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.212.b04-0.el7_6.x86_64
export PATH=$PATH:$JAVA_HOME/bin

安装maven
https://www-us.apache.org/dist/maven/maven-3/3.6.0/binaries/apache-maven-3.6.0-bin.tar.gz 

MAVEN_HOME=/usr/local/maven3
export MAVEN_HOME
export PATH=${PATH}:${MAVEN_HOME}/bin
    

4.让修改及时生效
source /etc/profile
5.配置完成后,使用java -version来检查是否配置成功

# tomcat启动慢的原因
https://www.cnblogs.com/jie-fang/p/7211574.html

# centos7防火墙设置
https://www.cnblogs.com/moxiaoan/p/5683743.html

# zookeeper的配置
server.1=127.0.0.1:2888:3888
server.2=127.0.0.1:2889:3889
server.3=127.0.0.1:2890:3890
