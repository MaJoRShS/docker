FROM python:3
LABEL maintainer 'Lucas Rodrigues <destroyerOffAss.com.br>'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log


USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD [ "run.py" ]