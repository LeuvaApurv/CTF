
### ☛ `File`

* A command-line tool for file format identification information. 

* Usage is **`file [filename]`** .
	 ```
	 sudo apt install file
	 ```

### ☛[`Hex Editer`](https://hexed.it)

* An online tool that allows you to modify the hexadecimal and binary values of an uploaded file.
  
### ☛ [`File Signatures`](https://www.filesignatures.net/index.php?page=all)

* An online tool that allows you to verify file signatures. [Trusted list of file signatures](https://en.wikipedia.org/wiki/List_of_file_signatures).

### ☛ `Strings`

* A command-line tool to search for all plain-text strings in the file.

* Usage is **`strings -o [filename]`**.
	```
	sudo apt install strings
	```

### ☛ `Binwalk`

* A command-line tool to carve files out of another file. 

* Usage to extract is **`binwalk -e [filename]`** and it will create a `_[filename]_extracted` directory. and also use this **`binwalk binwalk --dd='.*' [filename]`**.
	``` 
	sudo apt install binwalk
	```

### ☛ `Foremost`

* A command-line tool to carve files out of another file.
		
* Usage is **`foremost -i [filename]`** and it will create an `output` directory.
	```
	sudo apt install foremost
	```

### ☛`Exiftool`

* A command-line tool for matadata information. 

* Usage is **`exiftool [filename]`**.
	```
	sudo apt install exiftool
	```
