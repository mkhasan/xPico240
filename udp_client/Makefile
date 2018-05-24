CC := gcc
TARGET := udp_client
CFLAGS := -ggdb -Wall

all: build
build: bin/${TARGET}



bin/${TARGET}: obj/${TARGET}.o
	${CC} ${CFLAGS} ${LDFLAGS} $^ -o $@

obj/%.o: src/%.c
	${CC} -c ${CFLAGS} $< -o $@

clean:
	rm obj/*.o bin/* -rf

