# Print out file information about every.c file
# DANGER: * may not be directly used in a variable definitions
# DANGER: When * matches no files, it is left as it is
# (unless run in the wildcarrd function)

SRC = one.c two.c three.c

print: $(wildcard *.c) $(SRC)
	ls -la $?

$(SRC):
	touch $@

fclean:
	rm -f *.c

.PHONY: printfclean
