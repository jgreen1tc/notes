# Channel Status Word
Similar to [[PSW]] for the channel
- Double-word which contains 
	- the address of the [[CCW]]
	- status of the device
	- channel status flags
	- number of bytes to be read in or written out

| CSW Flags | CWW Address | Unit Status | Channel Status | Byte Count |
| --------- | ----------- | ----------- | -------------- | ---------- |
| 0-7       | 8-31        | 33-39       | 40-47          | 48-63      |   |

| CAW Flags | Channel Program Address |
| --------- | ----------------------- |
| 0-7       | 8-31                    |                         |
