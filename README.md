CTF
===============

> Leuva Apurv 

--------------------------

This repository, at the time of writing, will just host a listing of tools and commands that may help with CTF challenges.


Forensics & Steganography
-----------------------------

* `file`

	A command-line tool for file format identification information. Usage is `file [filename]` .

```
sudo apt install file
```

* [`hex editer`](hexed.it)

	An online tool that allows you to modify the hexadecimal and binary values of an uploaded file.
  
* [`file signatures`](https://www.filesignatures.net/index.php?page=all)

	An online tool that allows you to verify file signatures. [Trusted list of file signatures](https://en.wikipedia.org/wiki/List_of_file_signatures).

* `strings`

	A command-line tool to search for all plain-text strings in the file. Usage is `strings -o [filename]` .

```
sudo apt install strings
```

* `binwalk`

	A command-line tool to carve files out of another file. Usage to extract is `binwalk -e [filename]` and it will create a `_[filename]_extracted` directory. and also use this `binwalk binwalk --dd='.*' [filename]` .

```
sudo apt install binwalk
```

* `foremost`

	A command-line tool to carve files out of another file. Usage is `foremost -i [filename]` and it will create an `output` directory.

```
sudo apt install foremost
```
* `exiftool`

	A command-line tool for matadata information. Usage is `exiftool [filename]` .

```
sudo apt install exiftool
```

* `exiftool`

	A command-line tool for matadata information. Usage is `exiftool [filename]` .

```
sudo apt install exiftool
```

* [`TestDisk`](https://www.cgsecurity.org/wiki/TestDisk)

	A command-line tool, used to recover deleted files from a file system image. Handy to use if given a `.dd` and `.img` file etc.
	
* [`PhotoRec`](https://www.cgsecurity.org/wiki/PhotoRec)

	Another command-line utility that comes with `testdisk`. It is file data recovery software designed to recover lost files including video, documents and archives from hard disks, CD-ROMs, and lost pictures (thus the Photo Recovery name) from digital camera memory. PhotoRec ignores the file system and goes after the underlying data, so it will still work even if your media's file system has been severely damaged or reformatted. 
	
Image File Forensics
--------------------

[`AperiSolve`](https://aperisolve.fr/)
	Aperi'Solve is a platform which performs layer analysis on image (open-source).

