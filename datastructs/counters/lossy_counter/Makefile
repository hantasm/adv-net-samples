#Use the gcc compiler
CC=gcc
CFLAGS=-lm
LDFLAGS=-lm
RM=rm

#List of dependency files needed for compilation
DEPS=zipfgen.c lossycon.c lossy_test.c
OBJS=zipfgen.o lossycon.o lossy_test.o
TARGET=lossy_test

default:all

all:$(TARGET)

$(TARGET):$(OBJS)
	$(CC) -o $(TARGET) $(OBJS) $(LDFLAGS)

$(OBJS): $(DEPS)
	$(CC) -c $(DEPS) $(CFLAGS)

clean:
	$(RM) $(OBJS) $(TARGET)

rebuild:clean all
