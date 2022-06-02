# makefiles

## java

for a simple project directory structure

```make
SRCDIR = ./src
DOCDIR = ./doc
BINDIR = ./bin
JC = javac
JI = java
JCFLAGS = -g -d $(BINDIR) -cp $(SRCDIR)
JIFLAGS = -XX\:+ShowCodeDetailsInExceptionMessages -cp $(BINDIR)
MAINCLASS = main.Main
TESTCLASS = test.MainTest
.PHONY: clean docs opendocs
# add java specific suffix rule
.SUFFIXES: .java .class

all: run

.java.class:
	$(JC) $(JCFLAGS) $*.java

PROGCLASSES = $(SRCDIR)/main/*.java
TESTCLASSES = $(SRCDIR)/test/*.java

compile: $(PROGCLASSES:.java=.class)

run: clean compile
	$(JI) $(JIFLAGS) $(MAINCLASS)

test: $(TESTCLASSES:.java=.class)
	$(JI) $(JIFLAGS) $(TESTCLASS)

docs: $(PROGCLASSES)
	javadoc $(SRCDIR)/main/*.java $(SRCDIR)/vendor/*.java -d $(DOCDIR)

opendocs: docs
	xdg-open http://127.0.0.1:8005/
	python -m http.server 8005 -d $(DOCDIR) -b 127.0.0.1

clean:
	rm -rf $(BINDIR)/*
```
