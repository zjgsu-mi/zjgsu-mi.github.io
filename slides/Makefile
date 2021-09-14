SOURCE_DOCS := $(wildcard *.md)
EXPORTED_DOCS=\
			  $(SOURCE_DOCS:.md=.html)

%.html : %.md
	pandoc -t revealjs -s -V theme=white -o $@ $<

.PHONY: all clean

all : $(EXPORTED_DOCS)

clean:
	- $(RM) $(EXPORTED_DOCS)
