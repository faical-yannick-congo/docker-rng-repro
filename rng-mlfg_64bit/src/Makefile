#for GNU make

#DDEBUG = -O0 -g -ggdb -DDEBUG=1

CC = gcc -Wall -O3 -std=c99 -Wmissing-prototypes $(DDEBUG)
#CC = icc -Wall -O3 -std=c99 -Wmissing-prototypes $(DDEBUG)

all:  run

run:  run.c mlfg.o
	${CC} -o $@  run.c mlfg.o ${LINKOPT}

.c.o:
	${CC} -c $<

clean:
	rm -rf run *.o *~