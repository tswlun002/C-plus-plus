#This is a Makefile 
CC=g++                  #the compiler name
CCFLAGS=-std=c++2a      #flags passed to compiler
TARGET= extractor        #executable file
OBJECT= *.o             #binary file(s) 
SOURCE= *.cpp           #cc++ file(s)

#linking rules
$(TARGET): $(OBJECT)
	$(CC)	$(OBJECT)	-o	$(TARGET)	$(CCFLAGS)

#building rule
$(OBJECT): $(SOURCE)
	$(CC)	-c	$(SOURCE)	$(CCFLAGS)

#execution rule 
run:
	chmod +x frametester.sh;./frametester.sh

#clean rule
clean-image:
	rm -f *.pgm
	rm -f *.png
clean:
	@rm	-f	*.o 
	@rm	-f	extractor
	@rm	-f	*.pgm
	@rm	-f	*.png
	@rm	-f	-r	GENERATED_VIDEOS
	@rm	-f	*.mp4
