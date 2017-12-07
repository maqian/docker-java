FROM openjdk:9.0.1-11-jre

MAINTAINER Ma Qian<maqian258@gmail.com>

RUN curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/buster/set-sources-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/set-timezone-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/debian/set-locale-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/workarounds/master/docker/install-java-limit-memory' | sh

ENV TIMEZONE=Asia/Shanghai TZ=Asia/Shanghai \
    LANG=zh_CN.UTF-8 LC_ALL=zh_CN.UTF-8 LANGUAGE=zh_CN.UTF-8:zh:en_US:en
