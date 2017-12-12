FROM openjdk:8u151-jdk

MAINTAINER Ma Qian<maqian258@gmail.com>

RUN curl -sSL 'https://raw.githubusercontent.com/maqian/toolbox/master/debian/stretch/set-sources-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/toolbox/master/debian/set-timezone-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/toolbox/master/debian/set-locale-cn' | sh \
  && curl -sSL 'https://raw.githubusercontent.com/maqian/toolbox/master/sysfree/install-ejava' | sh \
  && apt-get install -y openjdk-8-dbg

ENV TIMEZONE=Asia/Shanghai TZ=Asia/Shanghai \
    LANG=zh_CN.UTF-8 LC_ALL=zh_CN.UTF-8 LANGUAGE=zh_CN.UTF-8:zh:en_US:en
