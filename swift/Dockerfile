FROM ubuntu:18.04

RUN apt-get update
RUN apt-get -y upgrade
RUN apt-get install -y clang libicu-dev wget git libcurl4-openssl-dev
RUN apt-get -y autoremove

RUN wget https://swift.org/builds/swift-5.1.4-release/ubuntu1804/swift-5.1.4-RELEASE/swift-5.1.4-RELEASE-ubuntu18.04.tar.gz -O swift.tar.gz
RUN mkdir swift
RUN tar -xzvf swift.tar.gz -C swift --strip-components 1
RUN mv swift /usr/local/bin/swift
RUN /usr/local/bin/swift/usr/bin/swift -version
