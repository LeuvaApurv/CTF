#  :sunglasses: CTF  :sunglasses:

> Leuva Apurv  |  August 21, 2020

--------------------------

This repository, at the time of writing, will just host a listing of tools and commands that may help with CTF challenges :wink:.


## Forensics & Steganography
-----------------------------

### ☛ `file`

A command-line tool for file format identification information. 

Usage is **`file [filename]`** .

 ```
 sudo apt install file
 ```

### ☛[`hex editer`](https://hexed.it)

An online tool that allows you to modify the hexadecimal and binary values of an uploaded file.
  
### ☛ [`file signatures`](https://www.filesignatures.net/index.php?page=all)

An online tool that allows you to verify file signatures. [Trusted list of file signatures](https://en.wikipedia.org/wiki/List_of_file_signatures).

### ☛ `strings`

A command-line tool to search for all plain-text strings in the file.
	
Usage is **`strings -o [filename]`**.

```
sudo apt install strings
```

### ☛ `binwalk`

A command-line tool to carve files out of another file. 
	
Usage to extract is **`binwalk -e [filename]`** and it will create a `_[filename]_extracted` directory. and also use this **`binwalk binwalk --dd='.*' [filename]`**.

``` 
sudo apt install binwalk
```

### ☛ `foremost`

A command-line tool to carve files out of another file.
		
Usage is **`foremost -i [filename]`** and it will create an `output` directory.

```
sudo apt install foremost
```

### ☛`exiftool`

A command-line tool for matadata information. 

Usage is **`exiftool [filename]`**.

```
sudo apt install exiftool
```

### ☛[`TestDisk`](https://www.cgsecurity.org/wiki/TestDisk)

A command-line tool, used to recover deleted files from a file system image. Handy to use if given a `.dd` and `.img` file etc.
	
### ☛[`PhotoRec`](https://www.cgsecurity.org/wiki/PhotoRec)

Another command-line utility that comes with `testdisk`. It is file data recovery software designed to recover lost files including video, documents and archives from hard disks, CD-ROMs, and lost pictures (thus the Photo Recovery name) from digital camera memory. PhotoRec ignores the file system and goes after the underlying data, so it will still work even if your media's file system has been severely damaged or reformatted. 
	

## Image File Forensics
--------------------

### ☛ [`AperiSolve`](https://aperisolve.fr/)
	
Aperi'Solve is an online platform which performs layer analysis on image. The platform also uses **zsteg, steghide, outguess, exiftool, binwalk, foremost and strings** for deeper steganography analysis. The platform supports the following images format: **.png, .jpg, .gif, .bmp, .jpeg, .jfif, .jpe, .tiff** ...

### ☛ `pngcheck`

A command-line tool for **checking** a PNG image file. Especially good for verifying checksums.
	
Usage is **`pngcheck [filename]`**.
```
sudo apt install pngcheck
```

### ☛ `steghide`
	
A command-line tool for steganography program that hides data in various kinds of image and audio files , only supports these file formats : **JPEG, BMP, WAV and AU**. but it’s also useful for extracting embedded and encrypted data from other files.
	
Usage is **`steghide info [filename]`**
and **`steghide extract -sf [filename]`**.	
```
sudo apt install steghide
```
	
### ☛ `zsteg`

A command-line tool that can detect hidden data in **png and bmp** files.
	
Usage is **`zsteg -a [filename]`**
```
sudo gem install zsteg
```

### ☛ `Stegsolve`
	
Sometimes there is a **message or a text hidden** in the image itself and in order to view it you need to apply some color filters or play with the color levels. 
	
Usage is **`./stegsolve`**
Just open the image with this tool and click on the  **`<`  `>`** buttons.
```
wget http://www.caesum.com/handbook/Stegsolve.jar -O stegsolve.jar
chmod +x stegsolve.jar
```

## Cryptography
----------------

### ☛ [`base32`](https://emn178.github.io/online-tools/base32_decode.html)

Base32 : The length of a **Base32-encoded** string is always a **multiple of 8**. Only these characters are used by the **encryption: `ABCDEFGHIJKLMNOPQRSTUVWXYZ234567 =` (no 0,1,8,9)**. The end with two times using the  **“=” character**. (this character is allowed in the end only)

### ☛ [`base64`](https://www.base64decode.org/)

Base64 : The length of a **Base64-encoded** string is always a **multiple of 4**. Only these characters are used by the **encryption: `ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=`**. The end with two times using the  **0,1,3,4,6 or “=” character**. It has a length greater than 40 to 60% of the original message.

### ☛ [`JSON Web Tokens`](https://jwt.io/#debugger-io)

JWT typically looks like `xxxxx.yyyyy.zzzzz` .

JSON Web Tokens consist of three parts separated by **dots (.)**, which are:

    Header
    Payload
    Signature

### ☛ [``]()



