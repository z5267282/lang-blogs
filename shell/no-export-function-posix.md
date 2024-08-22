POSIX compliance is sometimes difficult to work with in `dash`.  
Using `xargs` it is handy to use Shell functions with the `-exec` flag.  
This is better than having to write an individual file for shell functions.  
However as described in this [so post](https://stackoverflow.com/questions/1885871/exporting-a-function-in-shell)

```
In sh, it is not possible to export a function
```

. The full explanation is in this [other post](https://stackoverflow.com/questions/29239806/how-to-export-a-function-in-bourne-shell)

```
No. The POSIX specification for export lacks the -f present in bash that allows one to export a function.
A (very verbose) workaround is to save your function to a file and source it in the child script.
```

.