ls
./leviathan6
ltrace ./leviathan6 9999
gdb leviathan6
disassemble main
<+76>:    call   0x8048420 <atoi@plt>
<+84>:    cmp    -0xc(%ebp),%eax
<+20>:    movl   $0x1bd3,-0xc(%ebp)

0x1bd3 = 7123

^D
./leviathan6 7123
whoami
leviathan7
cat /etc/leviathan_pass/leviathan7
ahy7MaeBo9
