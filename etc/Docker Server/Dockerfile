FROM ubuntu:latest

#작성자 정보
LABEL name="Hwang Jeong Hwan"
LABEL maintainer=name
LABEL email="5832120@naver.com"

# apache2 설치시 사용자 입력 방지
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y apache2

EXPOSE 80

COPY index.html /var/www/html/

CMD service apache2 start
