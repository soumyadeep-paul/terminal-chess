FROM ubuntu:focal
# Installing required packages
RUN apt update -y \
	&& apt install -y stockfish python3-pip \
	&& pip3 install chs \
	&& sed -i 's/stockfish_10_x64_linux/\/usr\/games\/stockfish/' /usr/local/lib/python3.8/dist-packages/chs/engine/stockfish.py
# Creating user
RUN useradd -m chessplayer
USER chessplayer
# Setting terminal
RUN echo "export TERM=xterm"  >> ~/.bashrc
ENTRYPOINT ["chs"]
# Setting default level to 8, the toughest :)
CMD ["level=8"]
	


