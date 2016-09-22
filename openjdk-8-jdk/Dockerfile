FROM openjdk:8u102-jdk

MAINTAINER Ma Qian<maqian258@gmail.com>

RUN rm -rf /etc/apt/sources.list /etc/apt/sources.list.d/* \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/jessie/set-sources-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/jessie/set-timezone-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/jessie/set-locale-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/docker/java-limit-memory-installer' | sh

ENV TIMEZONE=Asia/Shanghai TZ=Asia/Shanghai \
    LANG=zh_CN.UTF-8 LC_ALL=zh_CN.UTF-8 LANGUAGE=zh_CN.UTF-8:zh:en_US:en \
    JAVA_OPTS="$JAVA_OPTS -XX:+PrintVMOptions -XX:+PrintCommandLineFlags"
