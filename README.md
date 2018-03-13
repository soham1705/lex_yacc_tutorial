# lex_yacc_tutorial
Tutorial for lex and yacc

Running lex (flex) for Windows users (basic example):
1. Create lex file with extension .l
2. Run `flex lexfile.l`. This creates a file called 'lex.yy.c'.
3. Run `gcc lex.yy.c -L "C:\MinGW\msys\1.0\lib\" -lfl`. The directory contains the 'libfl.a' file, which is necessary for running '-lfl'.
4. Run `.\a.exe` (or whatever the .exe file is called).
5. Enter input in corresponding lines, or redirect input from file. Note: input redirection '<' does not work in Powershell. Switch to Command Prompt to use that.

Running yacc (bison) for Windows users:
1. Create yacc file with extension .y
2. Run `bison -d yaccfile.y`. This creates two files called 'y.tab.c' and 'y.tab.h'.
3. Create lex file with extension .l and run as instructed above.
4. Run `gcc lex.yy.c y.tab.c -o output`, to create output file 'output.exe'.
5. Run `.\output.exe` (or whatever the .exe file is called).
6. Enter input in corresponding lines.

