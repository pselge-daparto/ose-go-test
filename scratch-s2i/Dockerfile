FROM alpine

LABEL  io.openshift.s2i.destination="/s2i"

COPY ./scratch-s2i/s2i /s2i

RUN chmod +x /s2i

RUN adduser goapp

USER goapp

CMD ["/s2i/usage"]