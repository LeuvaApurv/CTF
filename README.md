#  :sunglasses: CTF  :sunglasses:

> Leuva Apurv  |  August 21, 2020

--------------------------

This repository, at the time of writing, will just host a listing of tools and commands that may help with CTF challenges :wink:.


## Forensics & Steganography

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
		
Usage is **`foremost -i [filename]`** and it will create an `output` directory.

```
sudo apt install foremost
```

### ☛`Exiftool`

* A command-line tool for matadata information. 

Usage is **`exiftool [filename]`**.

```
sudo apt install exiftool
```

## Image File Forensics
--------------------

### ☛ [`AperiSolve`](https://aperisolve.fr/)
	
* Aperi'Solve is an online platform which performs layer analysis on image. 
* The platform also uses **zsteg, steghide, outguess, exiftool, binwalk, foremost and strings** for deeper steganography analysis. 
* The platform supports the following images format: **.png, .jpg, .gif, .bmp, .jpeg, .jfif, .jpe, .tiff** ...

### ☛ `Pngcheck`

* A command-line tool for **checking** a PNG image file. Especially good for verifying checksums.
* Usage is **`pngcheck [filename]`**.

```
sudo apt install pngcheck
```

### ☛ `Steghide`
	
* A command-line tool for steganography program that hides data in various kinds of image and audio files.
* Only supports these file formats : **JPEG, BMP, WAV and AU**. 
* But it’s also useful for extracting embedded and encrypted data from other files.
* Usage is **`steghide info [filename]`**
           **`steghide extract -sf [filename]`**.	
	   
```
sudo apt install steghide
```
	
### ☛ `Zsteg`

* A command-line tool that can detect hidden data in **png and bmp** files.
* Usage is **`zsteg -a [filename]`**.

```
sudo gem install zsteg
```

### ☛ `Stegsolve`
	
* Sometimes there is a **message or a text hidden** in the image itself and in order to view it you need to apply some color filters or play with the color levels. 
* Usage is **`./stegsolve`**
* Just open the image with this tool and click on the  **`<`  `>`** buttons.

```
wget http://www.caesum.com/handbook/Stegsolve.jar -O stegsolve.jar
chmod +x stegsolve.jar
```

## Cryptography

### ☛ [`Base32`](https://emn178.github.io/online-tools/base32_decode.html)

* The length of a **Base32-encoded** string is always a **multiple of 8**. 
* Only these characters are used by the **encryption: `ABCDEFGHIJKLMNOPQRSTUVWXYZ234567 =` (no 0,1,8,9)**. 
* The end with two times using the  **“=” character**. (this character is allowed in the end only)

### ☛ [`Base64`](https://www.base64decode.org/)

* The length of a **Base64-encoded** string is always a **multiple of 4**. 
* Only these characters are used by the **encryption: `ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=`**. 
* The end with two times using the  **0,1,3,4,6 or “=” character**. 
* It has a length greater than 40 to 60% of the original message.

### ☛ [`JSON Web Tokens`](https://jwt.io/#debugger-io)

* JWT typically looks like `xxxxx.yyyyy.zzzzz` .
* JSON Web Tokens consist of three parts separated by **dots (.)**, which are:
	```
	Header
	Payload
	Signature
	```
	
### ☛ [`Brainfuck`](https://www.splitbrain.org/_static/ook/)

* Brain Fuck is not a proper encryption system, but rather a programming language that has been obfuscated.
* Only these characters are used by the **encryption: `< > + * . , [ ]`**. 

### ☛ [`Ook!`](https://www.splitbrain.org/_static/ook/)

* Ook is a rewriting of the BrainFuck, an already obfuscated esoteric programming language, designed to be writable and readable by orang-utans (which would communicate by pronouncing the onomatopoeia 'ook, ook').
* The message consists of the words **Ook followed by `. (dot) or ? (question mark) or ! (exclamation mark)`**

	Brainfuck | Ook
	--------- | ----
	\+ | ..
	\- | !!
	\> | .?
	\< | ?.
	\[ | ! ?
	\] | ?!
	\. | !.
	\, | .!
	
### ☛ [`Phone Keypad`](https://www.dcode.fr/multitap-abc-cipher)
* Some messages may be hidden with a string of numbers, but really be encoded with old cell-phone keypads, like text messaging with numbers repeated:

![PhoneKeypad](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQSySxHjMFv80XWp74LZpfrnAro6a1MLqeF1F3zpguA5PGSW9ov)


