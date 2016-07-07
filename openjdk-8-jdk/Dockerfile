FROM java:openjdk-8u91-jdk

MAINTAINER Ma Qian<maqian258@gmail.com>

RUN rm -rf /etc/apt/sources.list /etc/apt/sources.list.d/* \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/jessie/set-apt-sources-cn' | sh \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/jessie/set-lang-cn' | sh \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/jessie/set-timezone-cn' | sh \
  && curl -fsSL 'https://raw.githubusercontent.com/maqian/workarounds/master/docker/java-limit-memory-installer' | sh

ENV TIMEZONE=Asia/Shanghai LANG=zh_CN.UTF-8 LC_ALL=zh_CN.UTF-8 LANGUAGE=zh_CN.UTF-8:zh:en_US:en
ENV JAVA_OPTS="$JAVA_OPTS -XX:+PrintVMOptions -XX:+PrintCommandLineFlags"
