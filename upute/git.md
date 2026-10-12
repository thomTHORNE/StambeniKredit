# Git

## Pravila

- Glavna grana je `main`. Remote je `origin` (adresa je u `git remote -v`).
- Commit radi nakon svake zaokružene izmjene dokumenata, a push kad korisnik to zatraži ili kad je to dogovoreni način rada.
- Poruke commita pisane su na hrvatskom, u jednom retku koji kaže što se promijenilo (npr. „Dodana ponuda banke X u usporedbu”). Po potrebi dodaj kratko objašnjenje u tijelu poruke.
- Ne koristi `--force`, ne prepisuj povijest i ne briši grane bez izričitog zahtjeva.
- Prije commita provjeri `git status` i dodaj samo namjerno izmijenjene datoteke. Pazi da ne dodaš binarne ni privremene datoteke.

## Prijava za push

- Ako push s korisnikova računala ne uspije zbog nedostatka podataka za prijavu, ne pokušavaj zaobilaziti autentifikaciju. Reci korisniku što se dogodilo i ponudi mogućnosti: da se sam prijavi (npr. Git Credential Manager ili token), ili, ako je dostupna ovlaštena veza s GitHubom u sesiji, da se push napravi preko nje.
- Lokalna kopija i `origin` moraju nakon pusha biti usklađeni (`git status` bez „ahead/behind”).
