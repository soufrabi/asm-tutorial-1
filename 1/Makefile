TARGET = main
SRC = main.s
OBJ = $(SRC:.s=.o)

$(TARGET): $(OBJ)
	ld -o $@ $^

$(OBJ): $(SRC)
	nasm -f elf64 -o $@ $<

clean:
	rm -f $(TARGET) $(OBJ)
	
