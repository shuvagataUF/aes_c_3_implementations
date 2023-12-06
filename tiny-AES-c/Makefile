#CC           = gcc
CC = aarch64-linux-gnu-gcc
CFLAGS = -g
APP_NAME = tiny-aes-c
BUILD_DIR = build

all: $(BUILD_DIR) tiny-aes-c

$(BUILD_DIR):
	mkdir -pv $(BUILD_DIR)

.PHONY:  lint clean

$(APP_NAME): test.c aes.h aes.c
	echo [CC] $@
	$(CC) $(CFLAGS) -o ./$(BUILD_DIR)/$@ $^

clean:
	rm -f *.OBJ *.LST *.o *.gch *.out *.hex *.map *.elf *.a $(BUILD_DIR)/$(APP_NAME)

test:
	make clean && make	&& ./$(BUILD_DIR)/$(APP_NAME)
