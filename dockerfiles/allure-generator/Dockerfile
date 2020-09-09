FROM timbru31/java-node:8-jre

RUN mkdir /allure
RUN mkdir /allure-results
RUN mkdir /allure-report
RUN mkdir /allure-config

RUN apt-get update && apt-get install unzip && apt-get install wget

RUN wget https://dl.bintray.com/qameta/maven/io/qameta/allure/allure-commandline/2.9.0/allure-commandline-2.9.0.zip
RUN unzip allure-commandline-2.9.0.zip -d /allure
RUN rm allure-commandline-2.9.0.zip
ENV PATH="/allure/allure-2.9.0/bin:${PATH}"
ENV ALLURE_CONFIG="/allure-config/allure.properties"
