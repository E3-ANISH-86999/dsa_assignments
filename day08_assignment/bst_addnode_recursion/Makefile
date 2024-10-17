TARGET=main
CC=gcc

$(TARGET).out: $(TARGET).o stack.o bst.o
	$(CC) $(TARGET).o stack.o bst.o -o $(TARGET).out

$(TARGET).o: $(TARGET).c
	$(CC) -c $(TARGET).c

stack.o: stack.c
	$(CC) -c stack.c

bst.o: bst.c
	$(CC) -c bst.c

run:
	./$(TARGET).out

clean:
	rm *.o *.out

.phony: run clean


