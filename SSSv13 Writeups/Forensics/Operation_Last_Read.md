# Operation Last Read

### RO:

Neobservând niciun flag real cu `exiftool` sau `strings`, recurgem la `binwalk`, cu care identificăm o arhivă `zip` dezarhivată automat odată cu extragerea folosind `binwalk -e`, care dezvăluie fișierul `pdf.txt`, care conține flagul `SSS{poti_sa_te_ascunzi_dar_nu_te_poti_ascunde}`

### EN:

As `exiftool` or `strings` don't have much to offer, we can use `binwalk` with which we identify a `zip` archive which is unarchived automatically via `binwalk -e`, leaving us with a `pdf.txt` file containing the flag `SSS{poti_sa_te_ascunzi_dar_nu_te_poti_ascunde}`.
