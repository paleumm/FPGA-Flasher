
# FPGA-Flasher
FPGA-Flasher For XC6SLX9

Download from [releases](https://github.com/ouoam/FPGA-Flasher/releases)

Automate flashing XC6SLX9 from *.bit file by drag and drop function

 1. Drag and drop your *.bit file
 2. Select your rom type which your want (Normal,Prom)
 3. Enter 


![Screenshot](https://raw.githubusercontent.com/thanatath/FPGA-Flasher/master/Screenshot.png)


# FPGA-Flasher for linux (Ubuntu 20.04, any distro that compatible with xc3sprog)

Install `xc3sprog` on Ubuntu 20.04

```bash
$ sudo apt update
$ sudo apt -y install xc3sprog
```

### Normal mode
```bash 
$ xc3sprog -c ftdi v -p 0 <path/to/file.bit>
```

### Prom mode

`spiflasherLX9.bit` from this repo

```bash
$ xc3sprog -c ftdi -v spiflasherLX9.bit
$ xc3sprog -c ftdi -v -R -p 0 -I <path/to/file.bit>
```


