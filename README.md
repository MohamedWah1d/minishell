# minishell
The main goal is to build a mini shell and execute some simple shell commands.
## shell.l and shell.y
l for lex and y for yacc
The goal for those two files is to make a parser for our minishell.
First we define a name for each symbol or text we want an action to happen after using  the lex
here is an example for the new line and the exit commands
```C
/n  {     
         return NEWLINE;
    }
    
"exit"  {     
         return exit;
    }
```C
