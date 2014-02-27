MODE= -O2 -Demx
decode.exe : decode.c musicout.c common.c common.h decoder.h huffman.h

HEDS =  common.h decoder.h huffman.h

OBJSD = decode.o musicout.o common.o huffman.o

LFLAG = 

PROGRAMD =  decode.exe

.c.o: $(HEDS)
	gcc -c $(MODE) $*.c

all: $(PROGRAM) $(PROGRAMD)

default: all


$(PROGRAMD) : $(OBJSD) $(HEDS)
	gcc -o $(PROGRAMD) $(LFLAG) $(OBJSD) -lm

clean:
	rm $(OBJSD)

veryclean:
	rm $(PROGRAM) $(OBJS)
