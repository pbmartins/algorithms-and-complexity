# makefile para o d�grafo/grafo din�mico
CC = gcc-5
CFLAGS = -ansi -Wall

OBJM = digraph.o pqueue_dijkstra.o
HEADERS = digraph.h pqueue_dijkstra.h

OBJECTS = $(OBJM) simdigraph.o pqueue_dijkstra.o
EXES = sdig

all:	$(EXES)

sdig:	simdigraph.o $(OBJM)
	$(CC) $(CFLAGS) simdigraph.o $(OBJM) -o sdig

$(OBJM):	$(HEADERS)

clean:
	rm -f $(OBJECTS) *~

cleanall:	clean
	rm -f $(EXES)
