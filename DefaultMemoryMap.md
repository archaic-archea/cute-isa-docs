## Memory
In the Cute ISA everything is mapped to memory, and thus can be accessed using memory.
So it might be useful to have a map of memory, and what generally goes there by default.

## Memory Locations
- `0x000-0x0FF` The primary stack. Most stack operations will be assumed to be taking place here, unless specified otherwise.
- `0x100-0x1FF` The secondary, or return, stack. When jumping, addresses will be default be stored here, and this is just a general use 2nd stack.
- `0x200-0x203` Instruction pointer. Points to the current instruction being used.
- `0x204-0x5FF` Default memory mapped IO range, see IO map for more details
- `0x600-0xFFFF_FFFF_FFFF_FFFF` Free memory. This can be allocated by the program. Info on this location will vary from machine to machine.

- `0x600` typically where the default program is loaded
