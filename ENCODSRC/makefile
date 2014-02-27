MODE = -O2 -Demx
encode.exe: encode.c musicin.c common.c common.h encoder.h subs.c psy.c tonal.c

HEDS = common.h encoder.h

OBJSD = encode.o musicin.o common.o subs.o psy.o tonal.o

LFLAG =

PROGRAMD = encode.exe

.c.o: $(HEDS)
	gcc -c $(MODE) $*.c

all: $(PROGRAM) $(PROGRAMD)

default: all


$(PROGRAMD) : $(OBJSD) $(HEDS)
	gcc -o $(PROGRAMD) $(LFLAG) $(OBJSD) -lm
