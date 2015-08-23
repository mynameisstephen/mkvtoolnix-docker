FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y wget
RUN wget -q -O - https://www.bunkus.org/gpg-pub-moritzbunkus.txt | sudo apt-key add -
RUN add-apt-repository "deb http://www.bunkus.org/ubuntu/trusty/ ./"
RUN apt-get -qy install mkvtoolnix && apt-get clean
CMD ["echo", "mkvinfo|mkvinfo-text|mkvmerge|mkvpropedit|mkvextract"]