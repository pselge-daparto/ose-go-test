FROM golang:1.12-alpine

LABEL   io.openshift.s2i.destination="/app" \
        io.openshift.s2i.scripts-url="image:///s2i"

COPY ./scratch-s2i/s2i /s2i

RUN chmod +x /s2i/* && \
    mkdir /app && \
    mkdir /.cache && \
    chown -R 1001 /app && \
    chown -R 1001 /.cache

USER 1001

CMD ["/s2i/usage"]