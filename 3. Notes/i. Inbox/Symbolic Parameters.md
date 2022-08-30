A variable that you intend to replace with a value at rune time, thus deferring the decision until necessary

When you invoke the procedure, you specify values for these parameters on the EXEC statement that invokes the procedure

In a procedure, a symbolic variable is written as an ampersand followed by 1-8 alphanumeric or national characters

```JCL
//STEP 1     EXEC PGM=IRLD11,PARM=&LOCATION
```
