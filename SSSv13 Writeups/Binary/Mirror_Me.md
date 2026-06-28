# Mirror Me

### RO:

Folosind `strings` și uitându-ne puțin la codul dezasamblat (folosind ghidra, IDA sau orice alt decompiler), ne dăm seama că trebuie să aflăm numerele naturale de trei cifre al căror produs să dea cel mai mare palindrom posibil. Din cultura noastră matematică, știm că acestea sunt 993 și 913 (sau facem un cod scurt de C/Python care să calculeze asta). Astfel, le trimitem separat de endline în instanța de netcat, care ne dă acces la un shell, de unde citim `/home/ctf/flag`.

### EN:

Using `strings` and looking at the dissasembled code, we see that we need to find the three-digit naturals that have the biggest palindrome possible as their product. Using our mathematical culture, we know that these are 993 and 913 (or we just write some quick C/Python code that calculates this). We send them separated by endlines, we get a shell and we can just read `/home/ctf/flag`
