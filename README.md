# modern-atari-8bit
Information on using an Atari 8-bit computer in modern times

There are a dizzying array of products that can be used to enhance the Atari 8-bit experience, and it can be a little confusing to figure out what all of them do -- particularly because much of the information is spread across forum posts from the last two decades!  I decided to write this up because it would have been useful to me a few years ago.

I've attempted to lay out here my understanding of the different categories, products inside that category, and links to more information on those products.  Note that some products are very versatile and will fall into multiple categories. 

Pull requests or issues are welcome to add to this or fix anything I have wrong, although no guarantees on how long it will take me to fix something. 

## Categories

### Device emulators

These emulate external devices, such as disk drives and communication devices, generally through the SIO port.  They're therefore limited to SIO speeds (19,200 bits per second standard, although 57,600 bps will sometimes work).

Top notch compatibility, because you're using an unmodified Atari, although a few copy protection schemes can still cause issues.

### Flash carts

These act like reprogrammable cartridges, meaning that you can map programs into cartridge memory ($A000-$BFFF) and run them from there.  This is great, because just like with real cartridges, there's no load time!  Near-perfect compatibility for cartridges (the Atari can't tell it's not a real cartridge).

### Mass storage attachments

These allow you to connect mass storage devices, such as compactflash or SD cards, to the Atari and access them like a disk drive.  In general, this works by either replacing the OS, or patching the stock Atari OS so that it accesses the mass storage device as D1: - D8: drives instead of a physical floppy drive.


### Replacement Operating Systems

These can be loaded into RAM, or can be put onto a (flash) ROM chip on the motherboard.  They enable additional features such as mass storage support (above).

### RAM upgrades

These allow adding additional memory (some as much as 4MB) to the Atari 8 bit computers.  16-bit address space and you can only reference 65,536 bytes of RAM?  Not a problem, we'll point a 4K section of memory at a thousand different places in expansion memory if we have to!

### Graphics upgrades

These allow video better output (RGB, S-Video, VGA, HDMI) and/or additional video modes (such as 80 characters or additional colors).

### Sound upgrades

You'd never guess from the category name, but these offer stereo and/or additional sound voices.

### Diagnostics

These allow you to diagnose issues with Atari 8-bit computers.

### Other

Anything that doesn't fall into one of the above categories.

## The devices

Here are some of the devices I know about, what category or categories they fall into, and some other facts and opinions.

1. [Fujinet](https://fujinet.online/what-is-fujinet/) (Device emulator) can emulate disk drives, cassette drives, modems, printers, and can also allow Atari applications to connect over the network.  The only issue I've found is that writes to ATX files aren't supported, so one of my favorite games (Alternate Reality) depends on this and doesn't run yet.
1. [A8Picocart](https://github.com/robinhedwards/A8PicoCart) (flash cart) is an inexpensive, easy to use flash cart.  Just drop files on the cart and go.  In addition to emulating a cartridge, it can also patch the OS and pretend to be a disk drive using ATR files, although that won't work for everything.
1. MyIDE and MyIDE-2 (flash cart, mass storage attachment)
1. MyBIOS
1. FAT32Loader 
1. SpartaDosX
1. 
