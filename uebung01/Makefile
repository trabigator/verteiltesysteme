CC=g++-4.9
CFLAGS=-c -Wall -std=c++0x
LDFLAGS=-fopenmp

all: main

main: main.o
	$(CC) main.o -o main $(LDFLAGS) -lpthread

main.o:
	§(CC) $(CFLAGS) main.cpp $(LDFLAGS)

test:
	./main

clean:
	rm -rf *.o main