
# Lab Report 3

**Command** `find`

**Alternates**

*The following commands were all found by going to the terminal and typing `man find`*

* `-size n[ckMGTP]` 

*Allows you to search for files based on their size, c for bytes, k for kilobytes, M for megabytes, G for gigabytes, T for terabytes , and P for petabytes. It's useful for locating files of a specific size or a range of size*

* `-type t` 

*Allows you to search for files based on their type, such as `d` for directories `f`for regular files. It's useful see all files of a type you have*

* `-newer file` 

*Allows you to search for files that are newer than a specified file. It's useful to track changes*

* `-iname pattern`

*Allows you search for files based on their name, however unlike `-name` it is case insensitive. It's useful for find files that may forgot what characters are uppercase or lowercase*

***

## Examples

**`-size n[ckMGTP]`**
* ``` # find ./technical -size +1M```
* ``` # find ./technical -size +1G```

**`-type t`**
* ``` # find ./technical -type d```
* ``` # find ./techincal -type f```

**`-newer file`**
* ``` # find ./techincal -newer file.txt```
* ``` # find ./techincal - newer doc.txt```

**`-iname pattern`**
* ``` # find ./technical -iname FiLe.tXt```
* ``` # find ./techincal -iname dOc.txT```

