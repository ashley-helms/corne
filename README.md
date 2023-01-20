# How To

Tested with qmk 0.16.9

## Install qmkmsys
[webpage](https://msys.qmk.fm/)


## Clone this repo

```
cd <qmk_source>/keyboards/crkbd/keymaps
git clone https://github.com/ashley-helms/corne.git
# Alternatively use ssh
```

## Flash the keyboard

Here you have to be careful to select the correct bootloader, which depends on
your selected microcontroller. [You can find more info here](https://docs.qmk.fm/#/flashing).

For DFU boards (Elite-C V4) use
```
qmk flash -kb crkbd -km ashley -bl dfu-split-left
qmk flash -kb crkbd -km ashley -bl dfu-split-right
```