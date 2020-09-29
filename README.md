# terminal-chess
### Prerequisite : 
Docker need to be installed on your system

### How does it work ? 
We are using chs python module from https://pypi.org/project/chs/ 

stockfish chess engine from https://stockfishchess.org/

### How to play ? 
docker run -it gajan1985/chessplay 

By default it runs with highst difficulty i.e 8. To play with reduced difficulty, you can run 

docker run -it gajan1985/chessplay level=1

Press ctrl-c to exit

### Playing instruction
In a chess board each row is marked with a number (1-8) and each column is marked with a letter (a-h). 

Knight=N

Queen=Q

King=K

Rook=R

Bishop=B

Pawn=No notation

![board image](/images/screen.png)

You can make a move by entering a command which is a combination of the piece and the destination. For eg to move your Knight from g1 to h3, you can enter Nh3 
