CC:=gcc
CFLAGS:=-Wall
LIB:=calculator.so
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)
LDFLAGS:=

.PHONY: all clean install uninstall

all: $(LIB)

$(LIB): $(OBJ)
	$(CC) $(CFLAGS) -o $(LIB) $^

install: $(LIB)
	install -m 644 math_functions.h $(DESTDIR)/$(PREFIX)/include

uninstall:

clean:
	rm -f $(LIB)
