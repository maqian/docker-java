FROM centos:7

MAINTAINER Ma Qian<maqian258@gmail.com>

RUN curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/set-sources-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/set-timezone-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/set-locale-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/centos/7/oracle-java-installer' | sh -s jre 8 131 11 d54c1d3a095b4ff2b6607d096fa80163 \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/docker/java-limit-memory-installer' | sh

ENV TIMEZONE=Asia/Shanghai TZ=Asia/Shanghai \
    LANG=zh_CN.UTF-8 LC_ALL=zh_CN.UTF-8 LANGUAGE=zh_CN.UTF-8:zh:en_US:en \
    JAVA_HOME=/usr/java/jre1.8.0_131 \
    MALLOC_ARENA_MAX=1
