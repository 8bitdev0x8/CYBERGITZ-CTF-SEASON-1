# CTF-Challenge–1

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#01the_hedgehog10_points">THE HEDGEHOG</a></li>
    <li><a href="#02steganosaurus30_points">STEGANOSAURUS</a></li>
    <li><a href="#03tomato_sauce30_points">TOMATO SAUCE</a></li>
    <li><a href="#04gollum_the_explorer20_points">GOLLUM THE EXPLORER</a></li>
    <li><a href="#05the_french_connection10_points">THE FRENCH CONNECTION</a></li>
    <li><a href="#06drop_the-bass10_points">DROP THE BASS!</a></li>
    <li><a href="#07its_sub_time10_points">ITS SUB TIME!</a></li>
    <li><a href="#08mein_kampf10_points">MEIN KAMPF</a></li>
    <li><a href="#09sms_of_the_internet10_points">SMS OF THE INTERNET</a></li>
    <li><a href="#10this_pandemic10_points">THIS PANDEMIC</a></li>
    <li><a href="#11data_of_data20_points">DATA OF DATA</a></li>
    <li><a href="#12morroco10_points">MORROCO</a></li>
    <li><a href="#13cardiogram20_points">CARDIOGRAM</a></li>
    <li><a href="#14stegnum_opus20_points">STEGNUM OPUS</a></li>
    <li><a href="#contributing">Contributing</a></li>
  </ol>
</details>

## 01.THE_HEDGEHOG–10_POINTS

### Sonic_visualizer
Sonic visualizer is a tool for viewing and analyzing the contents of audio files, however it can be helpful when dealing with audio steganography. You can reveal hidden shapes in audio files. [Website](https://www.sonicvisualiser.org/)

```bash
sudo apt-get install sonic-visualiser
```

```bash
flag{iwillbreakyourheart}
```

## 02.STEGANOSAURUS–30_POINTS

### Steghide

Steghide is a steganography program that hides data in various kinds of image and audio files , only supports these file formats : JPEG, BMP, WAV and AU. but it’s also useful for extracting embedded and encrypted data from other files.

It can be installed with apt however the [source](https://github.com/StefanoDeVuono/steghide) can be found on github.

```bash
steghide extract -sf <filename>
```
```bash
Base64 - ZmxhZ3t3b3d5MHVmMHVuZDF0fQ== 

Base64 Decoded - flag{wowy0uf0und1t}
```

## 03.TOMATO_SAUCE–30_POINTS

View Source using Web Inspector, Flag is hidden in CSS file.

```bash
flag{turnitleaveitstopformatit}
```

![alt text](https://github.com/8bitdev0x8/CYBERGITZ-CTF-SEASON-1/blob/main/03.TOMATO_SAUCE/Screenshot.png)


## 04.GOLLUM_THE_EXPLORER–20_POINTS

This flag doesn’t have a format and is one word.

### Exiftool


Sometimes important stuff is hidden in the metadata of the image or the file , exiftool can be very helpful to view the metadata of the files.
You can get it from [here](https://exiftool.org/)


#### Ubuntu, Debian, Mint, Kali


```bash
sudo apt install libimage-exiftool-perl
```

```bash
exiftool <filename>
```
GPS Cordinate data can be found in meta.


### Enter coordinates to find a place
On your computer, open [Google Maps](https://www.google.com/maps)
In the search box at the top, type your coordinates. Here are examples of formats that work:
Degrees, minutes, and seconds (DMS): 41°24'12.2"N 2°10'26.5"E
Degrees and decimal minutes (DMM): 41 24.2028, 2 10.4418
Decimal degrees (DD): 41.40338, 2.17403
You'll see a pin show up at your coordinates.

```bash
flag{naalumanikkkattu}
```

## 05.THE_FRENCH_CONNECTION–10_POINTS

Vigenère KEY : MOVIE 

Cipher : rzvo{xts_dvxaixpenzza}

Resource : [cyberchef](https://ctfacademy.github.io/crypto/cyberchef.htm)

```bash
flag{the_intouchables}
```

## 06.DROP_THE BASS!–10_POINTS

### Base64

Base64 is a group of binary-to-text encoding schemes that represent binary data (more specifically, a sequence of 8-bit bytes) in an ASCII string format by translating the data into a radix-64 representation. The term Base64 originates from a specific MIME content transfer encoding. Each non-final Base64 digit represents exactly 6 bits of data. Three 8-bit bytes (i.e., a total of 24 bits) can therefore be represented by four 6-bit Base64 digits.

Base64 Cipher : ZmxhZ3tXM19sMHYzX2hhY2tpbmd9

```bash
flag{W3_l0v3_hacking}
```


## 07.ITS_SUB_TIME!–10_POINTS

### Substitution Cipher

substitution cipher is a method of encrypting in which units of plaintext are replaced with the ciphertext, in a defined manner, with the help of a key; the "units" may be single letters (the most common), pairs of letters, triplets of letters, mixtures of the above, and so forth. The receiver deciphers the text by performing the inverse substitution process to extract the original message.


Alphabetical Substitution-

[Cipher](https://cryptii.com/pipes/caesar-cipher) : ysau{ekbhm0_ol_sgxt!}

KEY : AZERTYUIOPQSDFGHJKLMWXCVBN

```bash
flag{crypt0_is_love!}
```


## 08.MEIN_KAMPF–10_POINTS

Cipher : qbhbh zrmua irddh ljhmw uvh

The settings for the machine are:

Model: G-312

Reflector: UKW 11/26

Rotor 1: 2/12/6

Rotor 2: 1/17/16

Rotor 3: 3/12/1


```bash
flag{derflagistpeakyblinders}
```


## 09.SMS_OF_THE_INTERNET–10_POINTS

[Cipher](https://twitter.com/CSaintgits/status/1407709681976414211)

```bash
Ｃapｔｕrｅ the flａｇ cοnｔｅｓt ⅰs ａ сyｂersecｕｒⅰtｙ cｏmｐeｔiｔion 
```

### Twitter Secret Messages
Hide secret messages in your tweets (or any text) with steg-of-the-dump.js. [Site](https://holloway.nz/steg/)

```bash
flag{steganoispower}
```


## 10.THIS_PANDEMIC–10_POINTS


### Strings
Strings is a linux tool that displays printable strings in a file. That simple tool can be very helpful when solving stego challenges. Usually the embedded data is password protected or encrypted and sometimes the password is actaully in the file itself and can be easily viewed by using strings
It’s a default linux tool so you don’t need to install anything.

```bash
strings <filename>
```

```bash
flag{stay_h0m3_stay_saf3}
```


## 11.DATA_OF_DATA–20_POINTS

```bash
strings <filename>
```

```bash
flag{da_vinci_cod3}
```


## 12.MORROCO–10_POINTS

### Morse code 
Morse code is a method used in telecommunication to encode text characters as standardized sequences of two different signal durations, called dots and dashes, or dits and dahs. [DataBorder](https://databorder.com/transfer/morse-sound-receiver/)

```bash
flag{YOUR FLAG IS OPENSESAME}
```


## 13.CARDIOGRAM–20_POINTS

PNG embedded in PDF 

![alt text](https://github.com/8bitdev0x8/CYBERGITZ-CTF-SEASON-1/blob/main/13.CARDIOGRAM/image.ODV750.png)

```bash
flag{4023124842131283}
```


## 14.STEGNUM_OPUS–20_POINTS

### Zsteg
zsteg is a tool that can detect hidden data in png and bmp files.

install

```bash
zsteg <filename>
```

The source can be found on [github](https://github.com/zed-0xff/zsteg)

```bash
zsteg <filename>
```

```bash
flag{3v3rything_aint_cut3}
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update as appropriate.

8bitdev0x8 
