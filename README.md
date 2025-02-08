# os_loader

## Build 

```shell
nasm -f bin main.asm -o boot.img
```

## Run

Shorthand:
```shell
qemu-system-i386 -fda boot.img
```

To remove format warning, but not so concise:
```shell
qemu-system-i386 -drive file=boot.img,format=raw,index=0,media=disk
```
