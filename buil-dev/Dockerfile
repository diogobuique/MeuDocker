FROM python:3.6
LABEL maintainer 'Diogo Vieira Buíque <diogo.buique@itec.al.gov.br>'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python"]
CMD ["run.py"]
