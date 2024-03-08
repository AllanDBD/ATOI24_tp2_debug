CC=gcc
CFLAGS=-O3 -g

TARGET=main

all: $(TARGET)

libppm.so : ppm.c
		$(CC) $(CFLAGS) -fpic -shared $^ -o $@

main: main.c libppm.so
		$(CC) $(CFLAGS) $(LDFLAGS) main.c  -lppm -L. -Wl,-rpath=$(PWD) -o $@

clean:
		rm -fr $(TARGET) *.so
