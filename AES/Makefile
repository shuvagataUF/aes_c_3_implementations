#CC           = gcc
CC = aarch64-linux-gnu-gcc
CFLAGS = -g
APP_NAME = AES
BUILD_DIR = build

default: $(APP_NAME)

$(BUILD_DIR):
	mkdir -pv $(BUILD_DIR)

.PHONY:  lint clean

$(APP_NAME): gmult.c aes.c main.c
	echo [CC] $@
	$(CC) $(CFLAGS) -o ./$(BUILD_DIR)/$@ $^

clean:
	rm -f $(BUILD_DIR)/$(APP_NAME)

test:
	make clean && make	&& ./$(BUILD_DIR)/$(APP_NAME)
