FROM alpine

LABEL   io.openshift.s2i.destination="/s2i" \
        io.openshift.s2i.scripts-url="/s2i"

COPY ./scratch-s2i/s2i /s2i

RUN chmod +x /s2i


USER 1001

CMD ["/s2i/usage"]