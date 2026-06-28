# Black Hole

### RO:

Cu un `strings`, putem intui că ia un flag de undeva și doar îl trimite în `/dev/null`, ceea ce se și întâmplă. Folosind `ltrace -s 200 ./black_hole` putem găsi flagul `SSS{the_more_you_look_the_less_you_actually_see}`.

### EN:

Using `strings`, we can kind of guess that the binary takes some flag from god-knows-where and just drops it into `/dev/null`, which is actually what happens. Using `ltrace -s 200 ./black_hole` we can find the flag `SSS{the_more_you_look_the_less_you_actually_see}`.
