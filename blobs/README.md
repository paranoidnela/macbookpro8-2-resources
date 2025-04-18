# Blobs

These files come as-is: blobs extracted from roms or from my archives.

 - [`backuporigmacbookproa1286.BIN`](./backuporigmacbookproa1286.BIN): a dump of the stock firmware, probably obtained from badcaps. I've never seen the serial number in this dump, possibly mine
 - [`configold`](./configold): a very minimal hand written config, lacks payload configuration and blob configuration
 - [`.config`](./.config): a known working config, generated with menuconfig, not very readable but a good starting point
 - [`descriptor.bin`](./descriptor.bin): a flash descriptor extracted from the firmware dump, intended for the stock 8MB SPI, needs to be included in your coreboot tree (typically at: `3rdparty/blobs/mainboard/apple/macbookpro8_1/`)
 - [`me.bin`](./me.bin): the untouched management engine, extracted from the firmware dump, needs to be included in your coreboot tree (typically at: `3rdparty/blobs/mainboard/apple/macbookpro8_1/`)
 - [`pci8086,0116.rom`](./pci8086,0116.rom): this is the VGA optionrom that is mandatory for SeaBIOS and GRUB and needs to be included in your coreboot tree. Extracting this was quite difficult, but I don't remember why. I know for sure it's not what the 8,1 uses. I also remember getting tianocore to work with `libgfxinit` and not using the blob at all, but those fixes are probably not included here.
 