FROM nginx:1.25

# RUN apk add --no-cache ca-certificates

RUN rm -rf /etc/nginx/sites-enabled/* && rm -rf /etc/nginx/sites-available/*
COPY estage.conf /etc/nginx/sites-enabled/default.conf

EXPOSE 80

ENTRYPOINT [ "/docker-entrypoint.sh" ]

CMD ["nginx", "-g", "daemon off;"]