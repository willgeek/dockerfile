FROM alpine
MAINTAINER sayue2019@qq.com

# install mysql-client
RUN apk update && \
    apk add mysql-client

COPY init.sh /opt
RUN mkdir --mode 777 /opt/sqls && \
    chmod +x /opt
WORKDIR /opt

VOLUME /opt/sqls

#docker build -t sayue/mysql-client .
#docker run -it -v /sqls:/opt/sqls sayue/mysql-client /bin/bash -c 'sh ./init.sh bbs'
