# Operation 1337 Niffler

### RO:

Deschidem fișierul .pcap cu Wireshark și observăm în pachetul 21 mențiunea unui flag.txt. Așa că dorim să-l extragem.
Ne ducem la File > Export Objects > HTML și vedem o arhivă `08347211akamai.tar.gz`. După ce o dezarhivăm (nu este parolată), obținem fișierul `flag.txt`, conținând textul `SSS{prind_pachete_pe_retea}`.

### EN:

We can open the .pcap given with Wireshark and we can see in packet 21 that contains the mention of a `flag.txt`, so we would like to extract it.
We go to File > Export Objects > HTML and we see an archive. After saving and unarchiving it we obtain the `flag.txt` file, containing the string `SSS{prind_pachete_pe_retea}`.
