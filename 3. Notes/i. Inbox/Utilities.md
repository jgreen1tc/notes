A program that accomplishes a task that has to be done frequently by many people, such as:
- list files
- backup and restore files
- manage libraries
- sort files
- merge files

IEFBR14 - dummy program: all it does is "RETURN" (not a utility)
- used to pre-allocate or delete a non-VSAM data set:
```JCL
//ANY EXEC PGM=IEFBR14
//ANYFILE DD DSN=PREALLOCATED.FILE.HERE,DISP=(,CATLG),
//           UNIT=SYSDA,SPACE=(CYL(2,1))
```
more examples on pg 459