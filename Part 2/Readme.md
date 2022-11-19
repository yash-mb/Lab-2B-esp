# TODO:

1. Create a REPL to let you read and write RP2040 registers from a console. You should be able to:

2. select any 32-bit address to read/write (even if not a valid RP2020 address)

3. read/write any 32-bit value to this address

4. read/write using any of the atomic bit-setting aliases and a 32-bit mask


## REPL Video

The following demonstration video shows reading from and writing to a register directly. Atomic-bit setting can also implemented.

https://user-images.githubusercontent.com/73771085/202280796-6efb041b-b64c-434b-af71-99299a92152d.mp4

Here, when the user gives input as "r" followed by the address of the register (for e.g. d00000004 for address 0xd00000004), the program fetches the value of that register.

When user gives input as "w" to select write to register operation. User will then have to input the address of the register (for e.g. d00000010 for address 0xd00000010) followed by the value to be written into the register.
