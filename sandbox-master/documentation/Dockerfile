FROM alpine:3.12

EXPOSE 3010:3000

RUN mkdir -p /documentation

COPY builds/documentation /documentation/documentation
RUN chmod +x /documentation/documentation
COPY static/ /documentation/static

CMD ["/documentation/documentation", "-filePath", "/documentation/"]
