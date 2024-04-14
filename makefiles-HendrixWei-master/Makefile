CC = clang
CFLAGS = -c
LDFLAGS =

SRCS = driver.c file1.c file2.c
OBJS = $(SRCS:.c=.o)
TARGET = makefileAssignment

.PHONY: all clean

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(OBJS) -o $@

%.o: %.c headers.h
	$(CC) $(CFLAGS) $< -o $@

clean:
	rm -f $(OBJS) $(TARGET)
