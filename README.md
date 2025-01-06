# acse-solutions

## Reminder per l'esame
- Per ottenere la lunghezza di un array il cui puntatore sta nel registro $1:
  ```c
    t_symbol *array = getSymbol(program, $1);
    t_regID arraySize = getNewRegister(program);
    genLI(program, arraySize, array->arraySize);

- Le espressioni vengono rivalutate solo se eseguiamo nuovamente la semantic action associata all'espressione, quindi per rivalutare dobbiamo necessariamente separare il parsing in due (o più) parti e saltare ad un branch precedente alla semantic action
