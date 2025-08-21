Linux All Commands:
=============================
# Day05: Permissions

id: Display User identity
chmod: Changes file’s mode
umask: Set the default file permissions
su: Run a shell as another user
sudo: Execute a command as another user
chown: Change file’s owner
chgrp: Change a file’s group ownership
passwd: Change a user’s password
useradd: add the user using a built-in linux
adduser: adds the user using a perl script that internally useradd
groupadd: creates a new group



===========
# Day04: Escaping Characters

Backslash escape sequences
\a => Bell
\b => Backspace
\n => new line
\r => Carriage return
\t => Tab return


## Keyboard tricks:
- Cursor Movement Commands:
- Modifying Text:
- Killing and yanking (Cutting and Pasting) Text
- COMPLETION: 
- Using History
- Commands
- Seqence Action: 

history
history|less


===============

# Day03: SEEING THE WORLD AS SHELL SEES
## Expansion:
 * echo *
 * Pathname Expansion:
echo D*
echo *s
echo *t
echo /usr/*bin

* Tilde Expansion:
 echo ~
* Arithmetic Expansion: Shell allows you to expand arithmetics and the syntax would be $((expression))
 - Opertaors are: (+ - * / % **.)
* Brace Expansion:
 - echo Linux-{A,B,C,D}-version
 - echo Linux_{1..10}
 - echo {01..15}.txt
 - mkdir {2017..2020}-{01..12}
* Parameter Expansion:
 - echo $USER
 - echo $SHELL
* Command Substitution:
 - echo $(ls)
 - ls -l $(which mv)
* Quotes
 - touch "two Words.txt"
 - ls
* Supress Expansion:
 - echo *
 - echo '*'
 - echo {{01..10}}
 - echo '{{01..10}}'

==================================

date
cal
echo hello
cp 1.txt 2.txt
ping -c 4 google.com

ls
ls -a
ls -F
touch
cp
mv
rm
echo

sudo apt-get update
sudo apt install ncal
ping -c 10 arifulla.in
ping -c 4 google.com >> 1.txt

## What is softlink (symbolic link) in linux and what is hardlink?

Softlink: Create a hardlink

mkdir softest
cd softest
echo "welcome to Linux and practising softlink" > source.txt
cat source.txt
ln -s source.txt soure.file
cat source.file
ls
ls -la
rm source.txt
cat source.file

Hardlink:
mkdir hardtest
cd hardtest
echo "welcome to Linux -Practise Hardtesting" > source.txt
ln source.txt source.hardlink
cat source.hardlink
ls -al
rm source.txt
cat source.hardlink


What will be difference between hard link and normally copied file?

echo "welcomer to linux" > source
ls
ln source hardlink
cp source copiedfile
ls
ls -al
echo "Welcome to CSS" >> hardlink
cat hardlink
cat source
cat copiedfile


## Identifying Commands:

type ls
type cp
type ping
type type

which ls

help cd
mkdir --help
man ls
apropos partition


## Pipelines

ls -al /bin /usr/bin | sort | less
ls -al /bin /usr/bin/ | sort | uniq | wc -l

## tee

ls -al /bin /usr/bin | tee ls.txt | sort | uniq | wc -l