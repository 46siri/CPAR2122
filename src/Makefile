### Makefile ###

CC = gcc

CFLAGS = -Wall -O3 -ansi -D_GNU_SOURCE -g -std=c99

INCLUDE =-I include
OBJ := obj

SOURCES := $(wildcard $(SRC)/*.c)

OBJECTS := $(patsubst $(SRC)/%.c, $(OBJ)/%.o, $(SOURCES))

program1: bucketsort_paralelo.c
						gcc -o program1 bucketsort_paralelo.c

program2: bucketsort_sequencial.c
						gcc -o program2 bucketsort_sequencial.c

$(shell mkdir -p $(OBJ))

all : program1 program2

clean:
						rm -r $(OBJ)
						rm -f program1 program2
						rm -f gesval
