# Linux Shell

### Execute

Make command: `make`

### Commands Implemented:-

### <ins>cd</ins>

cd is used to change the current working directory to a specified folder.

**Flags Implemented :-**

- <ins>..</ins> <br>
  This flag enables user to navigate to parent directory.
- <ins>~</ins> <br>
  This flag enables user to navigate to home directory.

**Error Handling :-**

1. If you give more than one argument to cd .It will throw "Too many arguments error".
2. if you give more argument after cd ~ it will show error.

### <ins>echo</ins>

Displays a line of text on the terminal.

**Flags Implemented :-**

- <ins>-n</ins> <br>
  This flag doesn’t append a new line.
- <ins>--help</ins> <br>
  This flag lists all the executable commands.

**Error Handling :-**

1. If you don't give any argument to echo then it will print a new line character.
2. if echo --help and any other argument is given then it will show too many arguments.

### <ins>pwd</ins>

This command gives the present working directory of the shell.

**Flags Implemented :-**

- <ins>-L</ins> <br>
  This flag uses PWD from the environment, even if it contains symlinks.
- <ins>-P</ins> <br>
  This flag avoids all symlinks.

**Error Handling :-**

1. If you give more than two argument to pwd .It will throw "Too many arguments error".
2. If we get cwd problem then it will show error.

### <ins>date</ins>

Using this command, the user can print the system date and time.

**Flags Implemented :-**

- <ins>-u</ins> <br>
  Prints the coordinated universal time (UTC).
- <ins>-R</ins> <br>
  Outputs date and time in RFC 5322 format.

**Error Handling :-**

1. If you give more than two argument to date .It will throw "Invalid Command error".
2. If timeT gives NULL then it handles that part.

### <ins>cat</ins>

This command concatenates file and prints on the standard output.

**Flags Implemented :-**

- <ins>></ins> <br>
  This flag enables user to make a new file whose name is written after **>**.
- <ins>-n</ins> <br>
  This flag numbers all output lines.

**Error Handling :-**

1. If you give only one argument to cat .It will throw "Invalid Command error".
2. If it unable to open file then it will handle that and throw "File Does Not Exist error".

### <ins>ls</ins>

This command is used to list directory contents.

**Flags Implemented :-**

- <ins>-a</ins> <br>
  Using this flag, the command does not ignore entries starting with .
- <ins>-1</ins> <br>
  Using this flag, the command displays each entry in a new line.

**Error Handling :-**

1. If you give more than two argument to ls .It will throw "Invalid Command error".
2. If opendir() gives NULL then it will handle that part.

### <ins>rm</ins>

This command can be used to remove files or directories.

**Flags Implemented :-**

- <ins>-i</ins> <br>
  This flag prompts before every removal.
- <ins>-d</ins> <br>
  This flag is used to remove a directory.

**Error Handling :-**

1. If you give only one argument to rm .It will throws "Invalid Command error".
2. If you give a directory without -d flag then it throws "Cannot delete directory error". 

### <ins>mkdir</ins>

Using this command, we can make directories.

**Flags Implemented :-**

- <ins>-p</ins> <br>
  This flag creates all the directories recursively.
- <ins>-v</ins> <br>
  This flag prints a message for each created directory

**Error Handling :-**

1. If you give only one argument to mkdir .It will throw "Invalid Command error".
2. If there exist directory then it will throw error: "Directory already exists".
