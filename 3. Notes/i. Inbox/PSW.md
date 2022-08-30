# Program Status Word
- Tells the [[CPU]] 
	- where to find the next instruction to be executed
	- if the current program is privileged or not
	- what kind of interrupt just occurred
	- if DAT is turned on or off
	- etc
- If **Amode** bit in the PSW is on
	- Instruction is a 31 bit address (bits 33-63)
- If Amode=0
	- Instruction is a 24 bit address in bit 40-63 and bits 33-39 are ignored.
| PSW Flags (mode, storage key, condition code, etc) | Next instruction address |
| -------------------------------------------------- | ------------------------ |
| 0-63                                               | 64-127                   |
