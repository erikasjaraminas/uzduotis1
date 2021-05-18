CC:=gcc
BIN:=file_reader
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)

CPPFLAGS:=-I'$(shell pwd)'
CFLAGS:=-Wall

.PHONY: all clean

all: $(BIN)

$(BIN): $(OBJ)
	$(CC) $(CPPFLAGS) $(CFLAGS) -o $@ $^

clean:
	rm -rf $(BIN) $(OBJ)
