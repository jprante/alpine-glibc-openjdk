FROM fl.hbz-nrw.de/jprante/alpine-glibc

RUN mkdir -p /usr/lib/jvm && \
    wget -qO- "https://cdn.azul.com/zulu/bin/zulu11.41.23-ca-jre11.0.8-linux_x64.tar.gz" | tar -zx -C /usr/lib/jvm && \
    rm -f /usr/lib/jvm/zulu11.41.23-ca-jre11.0.8-linux_x64/lib/src.zip

ENV JAVA_HOME=/usr/lib/jvm/zulu11.41.23-ca-jre11.0.8-linux_x64 \
    PATH=$PATH:/usr/lib/jvm/zulu11.41.23-ca-jre11.0.8-linux_x64/bin
