# acse-solutions

## Carrellata di "trick" per il Lab
- Per accedere ad un array:
  ```c
    t_symbol *array = getSymbol(program, $1);
    t_regID arraySize = getNewRegister(program);
    genLI(program, arraySize, array->arraySize);
