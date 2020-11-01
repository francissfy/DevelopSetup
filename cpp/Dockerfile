FROM debian
LABEL Author="Shen Feiyu"
LABEL INFO="C++ Development"

# change apt source
RUN echo "deb http://mirrors.163.com/debian/ buster main non-free contrib" > /etc/apt/sources.list \
    && echo "deb http://mirrors.163.com/debian/ buster-updates main non-free contrib" >> /etc/apt/sources.list \
    && echo "deb http://mirrors.163.com/debian/ buster-backports main non-free contrib" >> /etc/apt/sources.list \
    && echo "deb-src http://mirrors.163.com/debian/ buster main non-free contrib" >> /etc/apt/sources.list \
    && echo "deb-src http://mirrors.163.com/debian/ buster-updates main non-free contrib" >> /etc/apt/sources.list \
    && echo "deb http://mirrors.163.com/debian-security/ buster/updates main non-free contrib" >> /etc/apt/sources.list \
    && echo "deb-src http://mirrors.163.com/debian-security/ buster/updates main non-free contrib" >> /etc/apt/sources.list

# install vim, c/c++, git, clang, gdb, cmake
RUN apt-get update \
    && apt-get install -y vim \
    && apt-get install -y build-essential \
    && apt-get install -y git \
    && apt-get install -y clang \
    && apt-get install -y gdb \
    && apt-get install -y cmake \
    && apt-get install -y ssh
    