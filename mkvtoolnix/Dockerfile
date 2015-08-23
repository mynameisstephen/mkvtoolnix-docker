FROM ubuntu:latest
RUN add-apt-repository "deb http://www.bunkus.org/ubuntu/trusty/ ./" && \
	wget -q -O - https://www.bunkus.org/gpg-pub-moritzbunkus.txt | sudo apt-key add - && \
	apt-get update && \
	apt-get install -qy mkvtoolnix && apt-get clean
CMD ["echo", "mkvinfo|mkvinfo-text|mkvmerge|mkvpropedit|mkvextract"]