
## Cryptography

### ☛ [`Base32`](https://emn178.github.io/online-tools/base32_decode.html)

* The length of a **Base32-encoded** string is always a **multiple of 8**. 

* Only these characters are used by the **encryption: `ABCDEFGHIJKLMNOPQRSTUVWXYZ234567 =` (no 0,1,8,9)**. 

* The end with two times using the  **“=” character**. (this character is allowed in the end only)

### ☛ [`Base64`](https://www.base64decode.org/)

* The length of a **Base64-encoded** string is always a **multiple of 4**. 

* Characters are used by **encryption: `ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=`**. 

* The end with two times using the  **0,1,3,4,6 or “=” character**. 

* It has a length greater than 40 to 60% of the original message.

### ☛ [`Binary`](https://www.rapidtables.com/convert/number/binary-to-ascii.html)

* Convert **Binary code** to **Text**:
	
	1. Get **binary byte**
	2. Convert **binary byte** to **decimal**
	3. Get character of **ASCII code** from **ASCII table**
	4. Continue with **next byte**

* Example : **Shizu** Translate to **`0101001101101000011010010111101001110101`**

### ☛ [`Hex`](https://www.rapidtables.com/convert/number/hex-to-ascii.html)

* Convert **Hex code** to **Text**:
	
	1. Get **hex byte**
	2. Convert **hex byte** to **decimal**
	3. Get character of **ASCII code** from **ASCII table**
	4. Continue with **next byte**
	
### ☛ [`Hex To File (binary)`](https://tomeko.net/online_tools/hex_to_file.php?lang=en)

* Convert **Hex code** to any type of **file**

### ☛ [`JSON Web Tokens`](https://jwt.io/#debugger-io)

* JWT typically looks like `xxxxx.yyyyy.zzzzz` .

* JSON Web Tokens consist of three parts separated by **dots (.)**, which are:
	1. Header
	2. Payload
	3. Signatur
	
* Example : 

	```
	eyJmbGFnIjoiU2hpenUiLCJBdXRob3IiOiJMZXV2YSBBcHVydiIsImFsZyI6IkhTMjU2In0.eyJnaXRodWIuY29tIjoiTGV1dmFBcHVydi9DVEYifQ.kIO1y_fvqszM0Lqdiz6AWXdlCjb0JmfMoQEYYdQHwmk
	```
		Output :

		HEADER:ALGORITHM & TOKEN TYPE
		{
			"flag": "Shizu",
			"Author": "Leuva Apurv",
			"alg": "HS256"
		}
		PAYLOAD:DATA
		{
			"github.com": "LeuvaApurv/CTF"
		}


### ☛ [`Tap Code`](https://cryptii.com/pipes/tap-code)

* **Tap code** is composed of a **single character repeated between 1 and 5 times**, a **separator (like /)** can be used, similar to the **Morse Code**.

* The message can be in the form of a **sound or light**, again repetitive.

* The **Tap code cipher** uses a grid of **letters, usually 5x5**, containing **25 of the 26 letters of the alphabet** (a letter is omitted, often the **J**, the **K** or the **Z**).

* Example :
	 \    | 1 | 2 | 3 | 4 | 5
	--    |-- |-- |-- |-- |--     
	**1** | A | B | C | D | E
	**2** | F | G | H | I | J/K
	**3** | L | M | N | O | P
	**4** | Q | R | S | T | U
	**5** | V | W | X | Y | Z

* **S** in position **4,3 (line 4 column 3)** corresponds to **4 then 3 DOTS** 

* **SHIZU** translates to **`.... ...  .. ...  .. ....  ..... .....  .... .....`**

### ☛ [`Brainfuck`](https://www.splitbrain.org/_static/ook/)

* **Brain Fuck** is not a proper **encryption system**, but rather a programming language that has been **obfuscated**.

* Only these characters are used by the **encryption: `< > + * . , [ ]`**. 

* Example : **Shizu**
	```
	+++++ ++++[ ->+++ +++++ +<]>+ +.<++ ++[-> ++++< ]>+++ ++.+. <++++ [->++
	++<]> +.--- --.<
	```

### ☛ [`Ook`](https://www.splitbrain.org/_static/ook/)

* **Ook** is a rewriting of the **BrainFuck**, an already obfuscated esoteric programming language, designed to be **writable and readable by orang-utans** (which would communicate by pronouncing the onomatopoeia 'ook, ook').

* The message consists of the words **Ook followed by `. (dot) or ? (question mark) or ! (exclamation mark)`**

* This is **two type** of encoded :
	
	1. **Ook** (Ook? Ook. Ook!)
	2. **Short Ook** (?.!) 

* **Brainfuck** to **Ook** to **Short Ook** :

	Brainfuck | Ook | Short Ook
	--------- | --- | ---------
	\+ | Ook. Ook. | ..
	\- | Ook! Ook! | !!
	\> | Ook. Ook? | .?
	\< | Ook? Ook. | ?.
	\[ | Ook! Ook? | !?
	\] | Ook? Ook! | ?!
	\. | Ook! Ook. | !.
	\, | Ook. Ook! | .!
	
* Example of Ook : **Shizu**
	```
	Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook! Ook? Ook! Ook! Ook. Ook? Ook. Ook. Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook. Ook? Ook. Ook?
	Ook! Ook. Ook? Ook. Ook. Ook. Ook. Ook! Ook. Ook? Ook. Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook. Ook! Ook? Ook! Ook! Ook. Ook? Ook. Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook? Ook. Ook? Ook! Ook. Ook? Ook. Ook. Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook. Ook! Ook. Ook. Ook. Ook! Ook. Ook? Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook. Ook. Ook! Ook? Ook! Ook! Ook. Ook? Ook. Ook. Ook. Ook.
	Ook. Ook. Ook. Ook. Ook? Ook. Ook? Ook! Ook. Ook? Ook. Ook. Ook! Ook. Ook!
	Ook! Ook! Ook! Ook! Ook! Ook! Ook! Ook! Ook! Ook! Ook. Ook? Ook. 
	```
* Example of Short Ook : **Shizu**
	```
	..... ..... ..... ...!? !!.?. ..... ..... ..... ..?.? !.?.. ..!.? .....
	....! ?!!.? ..... ...?. ?!.?. ..... ....! ...!. ?.... ..... !?!!. ?....
	....? .?!.? ..!.! !!!!! !!!!! .?.
	```

	
### ☛ [`Phone Keypad`](https://www.dcode.fr/multitap-abc-cipher)

* The ciphered message is made of numbers with **digits often repeated consecutively, between 1 and 3 times**, there a **few or none 1 or 0**.

* Example : **Shizu** Translate to **`7777 44 444 9999 88`**

	![PhoneKeypad](https://github.com/LeuvaApurv/CTF/blob/master/Image/Phone_Keypad.png)


### ☛ [`Keyboard Change Cipher`](https://www.dcode.fr/keyboard-change-cipher)

* The message is a **mono-alphabetic substitution**, no change in **index of coincidence**.

* The **QWERTY** and **AZERTY** keyboards (most commonly used) have several **common pairs (location, letter)** such as the letters **`ERTYUIOPSDFGHJKL`**

	Keybord | Alphabate
	------- | ---------  
	QWERTY | QWERTYUIOPASDFGHJKLZXCVBNM
	AZERTY | AZERTYUIOPQSDFGHJKLMWXCVBN
	DWORAK | PYFGCRLAOEUIDHTNSQJKXBMWVZ

### ☛ [`DVORAK Keyboard`](https://www.geocachingtoolbox.com/index.php?lang=en&page=dvorakKeyboard)

![DvorakKeybord](https://github.com/LeuvaApurv/CTF/blob/master/Image/Dvorak_KeyboardLayouts.jpg)

### ☛ [`Rot13`](https://rot13.com/)

* Online tool allows to **Rot1** to **Rot25**.


### ☛ [`Fernet`](https://asecuritysite.com/encryption/ferdecode)

* **Fernet** is a symmetric encryption method which makes sure that the message **encrypted cannot be manipulated/read** without the **key**.  
* It uses **URL safe encoding** for the **keys**. also **keys** look like **Base64**.
* Fernet uses **128-bit AES in CBC mode and PKCS7 padding**, with **HMAC using SHA256** for authentication.

* **`gAAAAA`** --> start with this chipher code use in **Fernet encryption**.

* Example : **Shizu**

	Key :  `WcZycMDlKc-Kv7JndqvKPgwx73zfET3PFg2C0i60nLw=`
	
	Token : `gAAAAABe4N-HmvkDc4JSybgwx9vGObpV6C10slGHOcfQHlReeo4GMjYmzFNCkykjwu8Wc8tzGBIwc9H8tYuGPH9YWq3pnLn4GA==`

	
### ☛ [`Malbolge`](http://malbolge.doleczek.pl/)

* **Malbolge**, invented by Ben Olmstead in 1998, is an esoteric programming language designed to be as difficult to program in as possible.

* An esoteric language that looks a lot **like Base85**... but **isn't**.

* Example : **Shizu**
	```
	'&%$#"!~}|{zyxwvutsrqponmlkjihgfedcba`_^]\[ZYXWVUTSRQPlNdibaf_dcbaZ~^]\>ZSw:
	9UTSRQ3IHMFj-,+*)('&%$#"!~}|{zyxwvutsrqponmlkjihgfedcba`_^]\[ZYXWVUTSRQPONML
	KJIHGFEDCB^]VUZYXWVOTMLpPONGLKDhU
	```

### ☛ [`Serpent`](https://www.tools4noobs.com/online_tools/decrypt/)

* **Serpent** is a symmetric key **block cipher** that was a finalist in the **Advanced Encryption Standard (AES)** contest, where it was ranked second to Rijndael.

* Example : 

		Chiper txt : `Jl/Q/lFSwCBJA5Fx4RikBg==`
		Key        : Nobi_21
		Mode       : ECB
	
		Output : Shizu



