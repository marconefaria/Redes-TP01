all:
	gcc -Wall -c common.c
	gcc -Wall -c handlers.c 
	gcc -Wall client.c common.o -o client
	gcc -Wall server.c common.o handlers.o -o server -lm
	gcc -Wall server.c common.o -lpthread -o server-mt
clean:
	rm common.o client server server-mt