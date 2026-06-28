# Pinpoint

### RO:

În codul dezasamblat identificăm scopul nostru: să suprascriem `v` pentru a obține un shell și a citi flagul. Identificăm adresa simbolului folosind `nm` (în formatul cerut de binar, `6295640`), iar cu o citire folosind `gdb`, vedem că valoarea inițială a lui `v` este `0x53535353` (`SSSS`), cea finală fiind `0x53585353` (`SXSS`). Astfel, adresa de scriere este `62955640+2=62955642`, iar valoarea `88` (`0x58`, care nu este acceptat de chall). Astfel, programul detectează schimbarea, ne alocă shellul și de acolo citim `/home/ctf/flag`.

### EN:

In the decompiled code, we identify our goal: to overwrite `v` in order to obtain a shell and read the flag. We determine the symbol’s address using `nm` (in the format required by the binary, `6295640`), and by inspecting it in `gdb`, we see that the initial value of `v` is `0x53535353` (`SSSS`), while the desired value is `0x53585353` (`SXSS`). Thus, the write address is `6295640 + 2 = 6295642`, and the value is `88` (`0x58`). After performing this write, the program detects the change, spawns a shell, and from there we read `/home/ctf/flag`.

