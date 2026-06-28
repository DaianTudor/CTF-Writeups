# The talker

### RO:

Notă: Depinzând de noroc, poți găsi binarul deja transmis prin SSH. Vom presupune că nu e acolo și îl vom pune noi manual.

Primim binarul `./the_talker`, pe care îl transmitem cu `scp -P 31302 ./the_talker connect@141.85.224.101:/home/connect/the_talker` folosind parola primită în enunț. Apoi ne logăm cu `ssh connect@141.85.224.101 -p 31302` și parola primită, pe două terminale. Pe primul terminal rulăm binarul, iar pe cel de-al doilea punem un listener cu `nc -u -lvp 4444`, iar după câteva secunde, primim flagul `SSS{the_talker_has_spoken}`.

Notă 2: Un exercițiu similar a fost propus la SSSv12 Essentials Final CTF.

### EN:

Note: Depending on luck, you can find the binary already transmitted via SSH. We will assume it is not there and we will put it manually.

We receive the binary `./the_talker`, which we transmit with `scp -P 31302 ./the_talker connect@141.85.224.101:/home/connect/the_talker` using the password provided in the statement. Then we log in with `ssh connect@141.85.224.101 -p 31302` and the provided password, on two terminals. On the first terminal we run the binary, and on the second we put a listener with `nc -u -lvp 4444`, and after a few seconds, we receive the flag `SSS{the_talker_has_spoken}`.

Note 2: A similar exercise appeared at SSSv12 Essentials Final CTF.

