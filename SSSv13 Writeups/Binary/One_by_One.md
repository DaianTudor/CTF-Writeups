# One by One

### RO:

Folosind `nm one_by_one` identificăm mai multe simboluri de tip „partX”, unde X este un nr. nat. de la 0 la 27. Ca să le citim, folosim GDB (GNU Debugger) și citim manual cu `x/1bx &partX` fiecare byte, care convertit în ASCII și pus în ordine dă flagul `SSS{a_chip_of_the_old_block}`

### EN:

Using `nm one_by_one` we see many "partX" symbols, where X is an integer from 0 to 27. To read them, we can use GDB and `x/1bx &partX` to read them manually. This way, by converting them with ASCII and putting them in order, we get the flag `SSS{a_chip_of_the_old_block}`.
