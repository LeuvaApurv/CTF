#  :sunglasses: CTF  :sunglasses:

> Leuva Apurv  |  June 10, 2020

--------------------------

This repository, at the time of writing, will just host a listing of online tools and commands that may help with CTF challenges :wink:


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


## Audio File Forensics
------------------------

### ☛ [`Spectral Analysis`](https://www.dcode.fr/spectral-analysis)

* Sometimes a **text (some letters)** or an **image (rather a silhouette)** is hidden in the **sound spectrum**.

* This site allows playback of **audio files** and analysis of sound **frequencies to render** it in different **colors and positioned on a sound frequency axis**.



## Cryptography



