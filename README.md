# CTF-Challenge–1

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
