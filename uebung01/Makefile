CC=g++-4.9
CL=g++
CFLAGS=-c -Wall -std=c++0x
LDFLAGS=-fopenmp

all: main matmult

main: main.o
	$(CC) main.o -o main $(LDFLAGS) -lpthread

main.o:
	$(CC) $(CFLAGS) main.cpp $(LDFLAGS)

matmult: matmult.o
	$(CL) matmult.o -o matmult

matmult.o:
	$(CL) $(CFLAGS) matmult.cpp $(LDFLAGS)

test:
	./main
	./matmult

clean:
	rm -rf *.o main matmult