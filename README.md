镜像说明
=======
Java已经马上就要进入1.9的时代，所以这里的镜像只有1.8以上的版本的JDK和JRE。openjdk和oracle-java都是使用比较广泛的jvm，分别对他们编写了Dockerfile。

openjdk的镜像继承自[官方openjdk镜像](https://hub.docker.com/_/java/)，oracle-java的镜像继承自[官方centos镜像](https://hub.docker.com/_/centos/)。

镜像列表
=======

* [openjdk-8-jdk](openjdk-8-jdk)
* [openjdk-8-jre](openjdk-8-jre)
* [oracle-java-8-jdk](oracle-java-8-jdk)
* [oracle-java-8-jre](oracle-java-8-jre)


openjdk-8-jdk
=============

1. 继承自官方镜像java:openjdk-8u91-jdk。
2. 添加aliyun镜像源。[使用脚本](https://github.com/maqian/workarounds/blob/master/debian/jessie/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/workarounds/blob/master/debian/jessie/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/workarounds/blob/master/debian/jessie/set-locale-cn)
5. 增加JVM内存限制。[使用脚本](https://github.com/maqian/workarounds/blob/master/docker/java-limit-memory-installer)


openjdk-8-jre
=============

1. 继承自官方镜像java:openjdk-8u91-jre。
2. 添加aliyun镜像源。[使用脚本](https://github.com/maqian/workarounds/blob/master/debian/jessie/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/workarounds/blob/master/debian/jessie/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/workarounds/blob/master/debian/jessie/set-locale-cn)
5. 增加内存限制。[使用脚本](https://github.com/maqian/workarounds/blob/master/docker/java-limit-memory-installer)


oracle-java-8-jdk
=================

1. 继承自基础自官方镜像centos:7
2. 添加aliyun镜像源。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/set-locale-cn)
5. 安装oracle-java官方jdk8u91，删除java安装目录无用的文件。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/oracle-java-installer)
6. 增加内存限制。[使用脚本](https://github.com/maqian/workarounds/blob/master/docker/java-limit-memory-installer)


oracle-java-8-jre
=================

1. 继承自基础自官方镜像centos:7
2. 添加aliyun镜像。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/set-locale-cn)
5. 安装oracle-java官方jre8u91，删除java安装目录无用的文件。[使用脚本](https://github.com/maqian/workarounds/blob/master/centos/7/oracle-java-installer)
6. 增加内存限制。[使用脚本](https://github.com/maqian/workarounds/blob/master/docker/java-limit-memory-installer)

