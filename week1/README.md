i learnt week 1 "Using files and Command"

`scp` `pwd` `cd` `rm` `ls` `less` `cat` `tree -L x` `(command options args)` `cp` `mv` `rm -r(recursively)` `rmdir(empty dir)` `mkdir` `touch`

after using `less` - `b -> beginning` | `g -> end` | `/word` 

`~`, `/`, `.`, `..` -  important dir's


`-a` -> hidden files

--------------------
i needed to find a python book but i forgot the name it was something with python and obviously it shouldbe a pdf file

so i applied this command 
```
find ~ -type f -iname "*python*.pdf"
```
which means find in the home dir type is filetype iname means it should be case insensitive the name shuold include *python*.pdf and ends with pdf extension
--------------------

## Remembering grep & find 
|   **grep**   |   **find**   | 
|--------------|--------------|
|   **grep = SEARCH for TEXT**   |   **find = SEARCH for FILES & DIRs**   |
|   grep [options] [pattern] [file]   |   find [path] [options] [patterns]   |
|   options:   |   options:   | 
|   -i -> ignore cases   |   -name -> search by name   |
|   -n -> show line numbers   |   -iname -> ignore case   |
|   -r -> recursive search   |   -type f/d -> file/dir   |
|   -v/-w/-x -> invert / word / line   |   -size +100M -> larger than 100 MB   |
|   -c -> count   |   -delete -> delete found files   |
|   -e -> multiple patterns   |
|   -l -> list filenames only   |
|   ex.     `grep -i "apple" fruits.txt`   |   **INCORRECT** `find . -iname -type f "*python*workout*book*.pdf"` ## incorrect bcz options needs arguments   |
|   `grep -e "hello" -e "world" hello.py`   |   **CORRECT**	 `find . -type f -iname "*python*workout*book*.pdf"` ## -type option getting f arg but -iname not   | 
|	|**CORRECT**   `find . -iname "*python*workout*book*.pdf" -type f` ## this is orrect too   |							
						        
## realisation
i am not sure but i think\n 

find = function(command)
**Command (`find`)** = function

**Options (`-type`, `-name`, `-size`)** = parameters

**Arguments (`f`, `"*.py"`, `"+100M"`)** = values passed to those parameters
```
find . -type f -name "*.py"
find (
     path='.',
     type='f',     ## type(f)
     name="*.py"   ## name("*.py")
     )

```
but some options are just flags which has true false values like -i -v for grep command so they dont need arguments

------------------------------------------

## Running multiple commands together 

|**Operator**|**Meaning**|
|------------|-----------|
|**`cmd1 && cmd2`**|if `cmd1` then `cmd2`|
|**`cmd1 \|\| cmd2`**|if **not** `cmd1` then `cmd2`|
|**`cmd1 ; cmd2`**|always run `cmd2`|
|**`(cmd1 && cmd2)`**|running command in a subshell|
|**`cmd1 \| cmd2`**|sen the output of `cmd1` into `cmd2`|

## xdg-open nano doesnt need cd bcz they accepts a path

### example 
```
xdg-open 21-127/infdesc.pdf
``` 
instead of 

```
cd 21-127 && xdg-open infdesc.pdf
```

---------------------------------------------

## Jobs, Man Pages, & Links

## Job Control Flow
```text   
             Ctrl+Z
                  │
                  ▼
             ┌─────────┐
             │ STOPPED │
             └─────────┘
              │       │
            fg│       │bg
              ▼       ▼
        ┌──────────┐  ┌──────────────┐
        │FOREGROUND│  │  BACKGROUND  │
        └──────────┘  └──────────────┘
              │              │
              │ Ctrl+C       │
              ▼              ▼
             EXIT           EXIT
```
`^C` -> Inturruption signal SIGINT to the program
`^Z` -> stop signal SIGTSTP the program
`^D` -> send EOF(Enf Of the File) condition to the REPL Program
if `^C` is ignored we can run `kill <PID(Process ID)>` or `kill %<job number>`
and to get PID `ps` or `ps u`

**REPL** Program is Read Eval Print Loop so if theres no more input REPL prgram will be finidhes there 

## Jobs vs Process
**Process** is core **OS operations** | **Job** is how **shell/zsh controls commands**
    
```text

                sleep 100
               /          \
              /            \
       OS's view          zsh's view
           │                  │
       PROCESS              JOB
       PID 19209            %1
       PROGRAM = sleep      COMMAND = sleep    

```

`man <command>` detailed | `<command> --help` in-short

## Symbolic Links(ln)

Create: ln -s TARGET (<-) LINK (create link symbolic LINK -> TARGET)
ex.
 
```bash
ln -s QuantCourse/Sem1/tools ~/tools
```

find all symbolic links: 
```bash
find ~ -type l

```
Inspecting a symbolic link:
```bash
ls -ld ~/tools

```
destroying:
 
```bash
rm ~/tools

```	

------------------------------------------------

## FILESYSTEMS

### Distributed Filesystems: 
```text
The Filesystem is distributed accross a network of machines 
```
ex. **cloud storage, network filesystem, servers, clusters, distributed systems**
---
### Filesystem Quota: 
```text
Maximum storage one user is allowed to have
```
---
### Permissions:
```text
what each category(owner/group/others) of users allowed to do. 
```
ex. in a **file permission string** rw-r-----

```markdown
		OWNER	GROUP	OTHERS
		 ↓       ↓       ↓
		rw-	r--	---
```

`r -> read | w -> write | x -> execute`
---

### ACL(Access Control List)

```text
a customized set of access rules for specific users/groups
```
---

