# SerMon

## import this repo into asm80.com

- click `Import repo from GitHub` button
- paste `https://github.com/jhlagado/SerMon` into the`Enter https GitHub link` text field.

## to run tests

- select the `main-test.z80` file
- press `Emulator [F10]` button

## to run app

- select the `main.z80` file
- press `Emulator [F10]` button

## to debug

- comment out line 1:

```asm
  ; .engine mycomputer
```

in `main.z80` or `main-test.z80` files

## Programming an 8K AT28C64B-15PU EEPROM

### truncate to 8192

head -c 8192 main.z80.bin > x.bin

### program to minipro

minipro -p AT28C64B -w x.bin
