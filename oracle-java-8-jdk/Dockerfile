FROM centos:7

MAINTAINER Ma Qian<maqian258@gmail.com>

RUN rm -f /etc/yum.repos.d/* \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/set-sources-cn' | sh \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/set-timezone-cn' | sh \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/set-locale-cn' | sh \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/java-installer' | sh -s jdk 8 92 14 \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/docker/java-limit-memory-installer' | sh

ENV TIMEZONE=Asia/Shanghai \
  LANG=zh_CN.UTF-8 LC_ALL=zh_CN.UTF-8 LANGUAGE=zh_CN.UTF-8:zh:en_US:en \
  JAVA_OPTS="-XX:+PrintVMOptions -XX:+PrintCommandLineFlags"
