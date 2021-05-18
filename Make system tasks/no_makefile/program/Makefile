CC:=gcc
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)
BIN:=calculator

CFLAGS:=-Wall
CPPFLAGS:=-I'$(shell pwd)'

.PHONY: all clean

all: $(BIN)

$(BIN): $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^

clean:
	rm -rf $(BIN) $(OBJ)
