CC=gcc
CFLAGS=-Wall

TARGET=lock

all: $(TARGET)

$(TARGET): lock.c
	$(CC) $(CFLAGS) -g -pthread -o $@ $<

clean:
	rm -f $(TARGET)