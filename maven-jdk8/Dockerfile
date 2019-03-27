FROM maven:3.6.0-jdk-8-alpine

# maven 阿里源
COPY ./settings.xml /root/.m2/
# ll 别名
RUN echo 'alias ll="ls -alh"' >> /root/.bashrc
