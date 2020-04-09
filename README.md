# learn_cobol
let's try this long-history language and make it fun during learning

## basic usage of cobol

Install COBOL compiler in ubuntu

```
~$ sudo apt-get install open-cobol
[sudo] password for yasen: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  gnucobol libcob4 libcob4-dev libgmp-dev libgmpxx4ldbl libncurses-dev
  libncurses5-dev
Suggested packages:
  gmp-doc libgmp10-doc libmpfr-dev ncurses-doc
The following NEW packages will be installed:
  gnucobol libcob4 libcob4-dev libgmp-dev libgmpxx4ldbl libncurses-dev
  libncurses5-dev open-cobol
0 upgraded, 8 newly installed, 0 to remove and 9 not upgraded.
Need to get 1,705 kB of archives.
After this operation, 7,268 kB of additional disk space will be used.
Do you want to continue? [Y/n] 
```

Once the installation is completed, use following commands to check the cobol compiler details:

```
~$ whereis cobc
cobc: /usr/bin/cobc /usr/share/man/man1/cobc.1.gz
```

```
~$ which cobc
/usr/bin/cobc
```

Compile the cobol program

Compile the HelloWorld which will create the HelloWorld executable.

```
~$ cobc -free -x -o cobol_helloworld-exe cobol_helloworld
~$ ls
cobol_helloworld  cobol_helloworld-exe
```

Note:
- -free - use free source format. Without this option cobol program requires certain format.
- -x - build executable program
- -o FILE - place the output file into the specified FILE.

Execute the cobol Program

Execute by mentioning the program name.

```
~$ ./cobol_helloworld-exe
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
Greetings from COBOL, HELLO WORLD!
```

Thanks [TheGeekstuff](http://www.ubuntugeek.com/how-to-install-cobol-compiler-and-run-cobol-program-in-ubuntu.html)