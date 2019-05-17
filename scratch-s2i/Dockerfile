FROM alpine

LABEL   io.openshift.s2i.destination="/app" \
        io.openshift.s2i.scripts-url="file:///s2i"

COPY ./scratch-s2i/s2i /s2i

RUN chmod +x /s2i/*
WORKDIR /app


USER 1001

CMD ["/s2i/usage"]