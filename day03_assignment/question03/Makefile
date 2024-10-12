TARGET=main
CC=gcc


$(TARGET).out: $(TARGET).o bubbleSort.o studMarksSort.o
	$(CC) $(TARGET).o bubbleSort.o studMarksSort.o -o $(TARGET).out 

$(TARGET).o: $(TARGET).c
	$(CC) -c $(TARGET).c

bubbleSort.o: bubbleSort.c
	$(CC) -c bubbleSort.c

studMarksSort.o: studMarksSort.c
	$(CC) -c studMarksSort.c

run:
	./$(TARGET).out

clean:
	rm *.o *.out
open:
	vim $(TARGET).c

phony: run clean open
