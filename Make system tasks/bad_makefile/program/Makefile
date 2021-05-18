CC:=gcc
CFLAGS:=-Wall
CPPFLAGS:=-I'$(shell pwd)'
OBJ:=main.o math_functions.o
BIN:=calculator

.PHONY: all clean

all: $(BIN)

$(BIN): $(OBJ)
	$(CC) $(CPPFLAGS) $(CFLAGS) -o $@ $^

clean:
	rm -f $(BIN) $(OBJ)
