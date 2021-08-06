FOO = foo
BAR = bar
FOOBAR := $(FOO) $(BAR)

all: $(FOOBAR)

$(FOOBAR):
	@echo $@ $(FOOBAR)

FOO = fooey
bar = barney

.PHONY: debug all
