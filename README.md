# loadenv.vim: load environment variables from shell setting

## USAGE

```vim
if executable('/usr/local/bin/bash') " Or your favorite shell
	call loadenv#load(
	\ '/usr/local/bin/bash -i -c __CMD__', " Use -i for interactive mode(read bashrc)
	\ ['PATH', 'JAVA_HOME']
	\ )
endif

" $PATH and $JAVA_HOME is set.
```
