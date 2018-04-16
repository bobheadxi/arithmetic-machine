# Arithmetic Machine
Pre-task for language team

```bash
$> clang main.c && ./a.out
```

## Instructions
`main.c` is a partial implementation of a small VM capable of performing simple arithmetic. To finsih the implementation, fill out the blanks labeled with `TODO`. We have given a correct implementation of `ADD` as an example for you, and a few macros for interacting with the VM you may find useful (`PUSH` and `POP`). More complete instructions can be found in the file.

some example programs:
Either `DCONST, 0x3F, 0xF0, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, PRINT, HALT` or `DCONST, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xF0, 0x3F, PRINT, HALT` should print `1.0`. Which one will work on your machine depends on your implementation of `DCONST` and/or the endianness of your machine.

`DCONST_2, ST1, DCONST_M1, LD1, DIV, PRINT, HALT` should print `-0.5`.

## Extra Credit
If you feel like this was too easy, feel free to add any capabilities you want to the VM. 
