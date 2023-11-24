#CC = gcc
CC = aarch64-linux-gnu-gcc
CFLAGS = -g
SOURCE_DIR = src
BUILD_DIR = build

all: $(BUILD_DIR) aes

$(BUILD_DIR):
	mkdir -pv $(BUILD_DIR)

aes:
	$(CC) $(CFLAGS) $(SOURCE_DIR)/main.c -o $(BUILD_DIR)/aes-in-c

clean:
	rm -rf $(BUILD_DIR)

.PHONY: all clean
