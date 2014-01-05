CC=gcc
CFLAGS=-g -Wall -Wextra

main: 	main.o interpreter.o parser.o tokenizer.o value.o
	$(CC) $(CFLAGS) -o interpreter main.o interpreter.o parser.o tokenizer.o value.o

main.o: main.c
	$(CC) $(CFLAGS) -c main.c

value.o: 	value.c
		$(CC) $(CFLAGS) -c value.c

tokenizer.o: 	tokenizer.c
		$(CC) $(CFLAGS) -c tokenizer.c

parser.o: 	parser.c
		$(CC) $(CFLAGS) -c parser.c

interpreter.o: 	interpreter.c
		$(CC) $(CFLAGS) -c interpreter.c

clean:
	rm *.o  