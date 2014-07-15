FROM ubuntu:latest

MAINTAINER tlacroix <tlacroix@octo.com>

RUN sudo apt-get update
RUN sudo apt-get install ruby -y
RUN gem install fakes3
VOLUME ["/mnt/fakes3_root"]

EXPOSE 4569
CMD ["fakes3", "-r", "/mnt/fakes3_root", "-p", "4569"]
