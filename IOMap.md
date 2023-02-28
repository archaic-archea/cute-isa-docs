## IO Memory
IO Memory in cute ISA is typically mapped into memory, around the range `0x204-0x5FF`.

## Memory Locations
- `0x000` Primary stack pointer.
- `0x004` Return stack pointer.
- `0x008` Primary stack offset. 
- `0x00A` Return stack offset.
- `0x100` Basic output device.
- `0x300` Base address for Simple Interrupt Controller.
