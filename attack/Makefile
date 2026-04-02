ifeq ($(OS),Windows_NT)
    # Windows-specific settings
    RM = del /F /Q
    EXT = .exe
else
    # Linux-specific settings
    RM = rm -f
    EXT =
endif

all: TwoTapAttack.o
	gcc -g -o TwoTapAttack TwoTapAttack.o

TwoTapAttack.o: TwoTapAttack.c
	gcc -g -c TwoTapAttack.c

.PHONY: clean

clean:
	$(RM) TwoTapAttack$(EXT) TwoTapAttack.o