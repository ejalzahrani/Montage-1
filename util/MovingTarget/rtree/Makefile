CC = gcc
CFLAGS = 

OBJECTS = card.o \
	index.o \
	mfmalloc.o \
	node.o \
	rect.o \
	split_q.o 

all: librtree.a

librtree.a: $(OBJECTS)
	ar rcv librtree.a $(OBJECTS)
	ranlib librtree.a

.c.o:
	$(CC) $(CFLAGS) -Wall -c $<

clean:
	rm -rf ./*.o ./*.a

