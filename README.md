镜像说明
=======
openjdk的镜像继承自[官方openjdk镜像](https://hub.docker.com/_/openjdk/)，oracle-java的镜像继承自[官方centos镜像](https://hub.docker.com/_/centos/)。

镜像列表
=======

* [openjdk-8-jdk](openjdk-8-jdk)
* [openjdk-8-jre](openjdk-8-jre)
* [openjdk-9-jdk](openjdk-9-jdk)
* [openjdk-9-jre](openjdk-9-jre)
* [oracle-java-8-jdk](oracle-java-8-jdk)
* [oracle-java-8-jre](oracle-java-8-jre)

openjdk-8-jdk
=============

1. 继承自官方镜像openjdk:8u151-jdk。
2. 添加中国镜像源。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/jessie/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-locale-cn)
5. 安装java启动脚本到/usr/local/bin/java。[查看脚本实现](https://github.com/maqian/toolbox/blob/master/bin/ejava)


openjdk-8-jre
=============

1. 继承自官方镜像openjdk:8u151-jre。
2. 添加中国镜像源。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/jessie/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-locale-cn)
5. 安装java启动脚本到/usr/local/bin/java。[查看脚本实现](https://github.com/maqian/toolbox/blob/master/bin/ejava)

openjdk-9-jdk
=============

1. 继承自官方镜像openjdk:9.0.1-jdk。
2. 添加中国镜像源。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/stretch/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-locale-cn)
5. 安装java启动脚本到/usr/local/bin/java。[查看脚本实现](https://github.com/maqian/toolbox/blob/master/bin/ejava)


openjdk-9-jre
=============

1. 继承自官方镜像openjdk:9.0.1-jre。
2. 添加中国镜像源。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/stretch/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/toolbox/blob/master/debian/set-locale-cn)
5. 安装java启动脚本到/usr/local/bin/java。[查看脚本实现](https://github.com/maqian/toolbox/blob/master/bin/ejava)

oracle-java-8-jdk
=================

1. 继承自基础自官方镜像centos:7
2. 添加aliyun镜像源。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/set-locale-cn)
5. 安装oracle-java官方jdk8u152，删除java安装目录无用的文件。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/install-oracle-java)
6. 安装java启动脚本到/usr/local/bin/java。[查看脚本实现](https://github.com/maqian/toolbox/blob/master/bin/ejava)


oracle-java-8-jre
=================

1. 继承自基础自官方镜像centos:7
2. 添加aliyun镜像源。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/set-sources-cn)
3. 修改timezone为Asia/Shanghai。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/set-timezone-cn)
4. 修改locale为zh_CN.UTF-8。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/set-locale-cn)
5. 安装oracle-java官方jre8u152，删除java安装目录无用的文件。[使用脚本](https://github.com/maqian/toolbox/blob/master/centos/7/install-oracle-java)
6. 安装java启动脚本/usr/local/bin/java。[查看脚本实现](https://github.com/maqian/toolbox/blob/master/bin/ejava)

