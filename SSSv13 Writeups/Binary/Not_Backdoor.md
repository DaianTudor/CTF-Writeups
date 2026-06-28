# Not Backdoor

### RO:

Aparentul nostru fișier .exe este de fapt un binar ELF într-o arhivă, unde avem o funcție `FUN_004006b6` (așa apare în ghidra, nu știu dacă e persistentă treaba asta, teoretic da, pentru că se folosește de adresa la care începe funcția) unde avem un șir de caractere `local_38`. Observăm că funcția ia acest șir, îl XOR-ează cu o valoare dată ca parametru. Ce mai observăm e că șirul începe cu trei valori egale (`0x3c`), ceea ce ne împinge să XOR-ăm cu `0x6f` pentru a obține `SSS` ca primele trei caractere, astfel obținând flagul `SSS{pr3tty_c0nvoluted_fl4g}`.

Notă: Prin dezarhivare și dat brute-force putem ajunge la același rezultat.

### EN:

Our .exe file is, in fact, an archived ELF. By opening it in ghidra, we can find the function `FUN_004006b6`, where we also find a string `local_38`. We see two things: the function XORs the string with a parameter and the string starts with three `0x3c`, which makes us want to XOR the whole string with `0x6f`, which gives us the `SSS{pr3tty_c0nvoluted_fl4g}`.
