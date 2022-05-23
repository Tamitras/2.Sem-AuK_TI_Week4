#modify commands and folders here if necessary
BIN = ./bin/
SRC = ./src/
INC = ./src/
RM = rm -f
CC = gcc -g

all: clean $(BIN)dhbwstudent.o $(BIN)dhbwstudentlist.o $(BIN)dhbwstudenttree.o $(BIN)dhbwstudentmap.o $(BIN)dhbwtest.o $(BIN)datastructures.o $(BIN)datastructures

clean:
	$(RM) $(BIN)*.o $(BIN)*.exe

$(BIN)dhbwstudent.o: $(SRC)dhbwstudent.c $(INC)dhbwstudent.h
	$(CC) -o $(BIN)/dhbwstudent.o -c $(SRC)dhbwstudent.c 

$(BIN)dhbwstudentlist.o: $(SRC)dhbwstudentlist.c $(INC)dhbwstudentlist.h
	$(CC) -o $(BIN)/dhbwstudentlist.o -c $(SRC)dhbwstudentlist.c 


$(BIN)dhbwstudenttree.o: $(SRC)dhbwstudenttree.c $(INC)dhbwstudenttree.h
	$(CC) -o $(BIN)/dhbwstudenttree.o -c $(SRC)dhbwstudenttree.c 

$(BIN)dhbwstudentmap.o: $(SRC)dhbwstudentmap.c $(INC)dhbwstudentmap.h
	$(CC) -o $(BIN)/dhbwstudentmap.o -c $(SRC)dhbwstudentmap.c 

$(BIN)dhbwtest.o: $(SRC)dhbwtest.c $(INC)dhbwtest.h
	$(CC) -o $(BIN)/dhbwtest.o -c $(SRC)dhbwtest.c

$(BIN)datastructures.o: $(SRC)datastructures.c 
	$(CC) -o $(BIN)/datastructures.o -c $(SRC)datastructures.c

$(BIN)datastructures: $(BIN)datastructures.o
	$(CC) -o $(BIN)datastructures $(BIN)datastructures.o $(BIN)dhbwtest.o $(BIN)dhbwstudent.o $(BIN)dhbwstudentlist.o $(BIN)dhbwstudenttree.o $(BIN)dhbwstudentmap.o

