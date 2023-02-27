### SIC
In the cute isa we need interrupts, so we by default have an interrupt line, and hand off the rest to an interrupt controller, in this case the SIC to handle interrupts and interactions.

### Map

- `Base + 0x00` Jump Address: The address jumped to when an interrupt is triggered.
- `Base + 0x04` Cause: The cause of the interrupt, in the form of an unsigned 32 bit integer, where the upper most bit being set means its an exception
- `base + 0x08` Return Address: Where the address to return to is stored, you must load this in the stack before returning
