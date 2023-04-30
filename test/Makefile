main:
	gcc -c -Wall -Werror -fpic ./lib/cat.c -o ./lib/cat.o
	gcc -shared -o ./shared-libraries/libcat.so ./lib/cat.o
	gcc -L./shared-libraries -Wl,-rpath=./shared-libraries -Wall -o test new_Busybox.c -lcat
