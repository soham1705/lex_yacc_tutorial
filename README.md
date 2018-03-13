# lex_yacc_tutorial
Tutorial for lex and yacc

Running lex (flex) for Windows users:
1. Create lex file with extension .lex
2. Run `flex lexfile.lex`. This creates a file called _lex.yy.c_.
3. Run `gcc lex.yy.c -L "C:\MinGW\msys\1.0\lib\" -lfl`. The directory contains the 'libfl.a' file, which is necessary for running '-lfl'.
4. Run `.\a.exe`.
5. Enter input in corresponding lines, or redirect input from file. Note: input redirection '<' does not work in Powershell. Switch to Command Prompt to use that.
