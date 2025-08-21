# Linux All Commands:
=============================
# Day01: Linux Foundation Series
## Linux – The Operating System
  * Distributions Different types
## Layers of Abstraction in Linux
 * Explain about artcitecture
## Shell and Terminal
## Creating Linux Instances on the cloud : For lab practise
  * Done
## Linux Commands : basics
## Linux directory hierarchy
## Environment and Shell variables
## Using Text Editors

# Day02:

## Linux Useful utils
 * Which Shell are you running?
 * Aborting and suspending the execution of linux programs
 * Redirecting output of a command to a file instead of terminal (stdout)
 * Common Errors
 * What is softlink (symbolic link) in linux and what is hardlink? 
 * What will be difference between hard link and normally copied file?
 * Identifying Commands
   * type ls
   * which ls
   * Getting a Commands Documentation
     - help cd
     - mkdir --help
     - man ls
     - apropos partition

## Pipelines:
  ls -al /bin/usr/bin | sort | less
  ls -al /bin/usr/bin/ | sort | uniq | wc -l

## tee
ls -al /bin /usr/bin | tee ls.txt | sort | uniq | wc -l

# Day03: SEEING THE WORLD AS SHELL SEES

## Expansion:
 * echo *
 * Pathname Expansion:
    - echo D*
    - echo *s
    - echo *t
    - echo /usr/*bin

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