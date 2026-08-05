i learnt week 1 "Using files and Command"

scp pwd cd rm ls less cat tree -L x (command options args) cp mv rm -r(recursively) rmdir(empty dir) mkdir touch

after using less b -> beginning | g -> end | /word 

~ / . .. important dir's


-a -> hidden files

--------------------
i needed to find a python book but i forgot the name it was something with python and obviously it shouldbe a pdf file

so i applied this command find ~ -type f -iname "*python*.pdf"
which means find in the home dir type is filetype iname means it should be case insensitive the name shuold include *python*.pdf and ends with pdf extension
--------------------

## Remembering grep & find 
 
grep = SEARCH for TEXT                      |   find = SEARCH for FILES & DIRs
                                            |
grep [options] [pattern] [file]             | find [path] [options] [patterns]
                                            |
options: -i -> ignore cases                 |options: -name -> search by name
	 -n -> show line numbers            |	      -iname -> ignore case
	 -r -> recursive search             | 	      -type f/d -> file/dir
	 -v/-w/-x -> invert / word / line   |         -size +100M -> larger than 100 MB
	 -c -> count                        |         -delete -> delete found files
	 -e -> multiple patterns            |
	 -l -> list filenames only          |

ex.     grep -i "apple" fruits.txt          |        *INCORRECT* find . -iname -type f "*python*workout*book*.pdf" ## incorrect bcz options needs arguments
	grep -e "hello" -e "world" hello.py |	     *CORRECT*	 find . -type f -iname "*python*workout*book*.pdf" ## -type option getting f arg but -iname not 
						     *CORRECT*   find . -iname "*python*workout*book*.pdf" -type f ## this is orrect too							
						        
## realisation
i am not sure but i think options[-type, -name, -size] are just like parameters to the command(function) find which needs a argument(values)[f, "*.py", "+100M"]

find . -type f -name "*.py"
find (
     path='.',
     type='f',     ## type(f)
     name="*.py"   ## name("*.py")
     )


but some options are just flags which has true false values like -i -v for grep command so they dont need arguments
