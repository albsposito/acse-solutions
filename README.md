# acse-solutions

## Carrellata di "trick" per il Lab
- Per ottenere la lunghezza di un array il cui puntatore sta nel registro $1:
  ```c
    t_symbol *array = getSymbol(program, $1);
    t_regID arraySize = getNewRegister(program);
    genLI(program, arraySize, array->arraySize);
