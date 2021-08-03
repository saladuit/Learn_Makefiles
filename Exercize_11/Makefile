objects = foo.o bar.o all.o
all: $(objects)

# These files are compiled via implicit rules
# Syntax - targets ...: targets-pattern: prereq-patterns ...
# In the case of the first target, foo.o,
# the target-pattern matches foo.o and sets the "stem" to be "foo".
# It then replaces the '%' in prereq-pattern with that stem
$(objects): %.o: %.c

all.c:
	echo "int main() { return (0); }" > all.c

%.c:
	touch $@

clean:
	rm -f *.c *.o all
