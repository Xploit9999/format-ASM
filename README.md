### DESCRIPTION

This script format disk(s) for ASM disk groups. Its only works for Solaris O.S

### USAGE

    -r  You can specify a range for example: 10-50 or it work as a single number.
    -d  You must specify the nomenclature of device, for example: starts with c0d or c1d or c2d and so on..
        to know what type of nomenclature of device has you, try to do an echo | format 
        Example output:

        AVAILABLE DISK SELECTIONS:
           0. c1d0 <QEMU HAR-QM0000-0001-20.00GB> # <- as you can see its start with c1d and 0 its the id of the disk.
              /pci@0,0/pci-ide@1,1/ide@0/cmdk@0,0

### IMPORTANT NOTE:

    [ ! ] Posible things that you may know if you see this:
    [ x ] You must run this script as a root.
    [ x ] This script was made only for Solaris O.S 
    [ x ] You entered an invalid parameter or are missing one.
    [ - ] This can be showed with the flag -h

### EXAMPLE:

    1. Format disk from 20 to 50 with nomenclature of device c0d
```vim    
    ./ASM_format -r 20-50 -d c0d
```

    2. Format a single disk with number 10 with nomenclature of device c2d
```vim    
    ./ASM_format -r 10 -d c2d
```
