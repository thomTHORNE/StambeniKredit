# Git

## Pravila

- Glavna grana je `main`. Remote je `origin` (adresa je u `git remote -v`).
- Nakon svake zaokružene izmjene dokumenata napravi commit i push.
- Poruke commita pisane su na hrvatskom, u jednom retku koji kaže što se promijenilo (npr. „Dodana ponuda banke X u usporedbu”). Po potrebi dodaj kratko objašnjenje u tijelu poruke.
- Ne koristi `--force`, ne prepisuj povijest i ne briši grane bez izričitog zahtjeva.
- Prije commita provjeri `git status` i dodaj samo namjerno izmijenjene datoteke. Pazi da ne dodaš binarne ni privremene datoteke.

## Gdje se radi

- Repozitorij se vodi samo na GitHubu. Korisnik nema lokalnu kopiju na svom računalu i ne treba je usklađivati.
- Na početku rada dohvati repozitorij s GitHuba u radno okruženje (clone ili pull), radi izmjene ondje, napravi commit i push.
- Nakon pusha radna kopija i `origin` moraju biti usklađeni (`git status` bez „ahead/behind”).
- Ako push ne uspije zbog nedostatka podataka za prijavu, ne pokušavaj zaobilaziti autentifikaciju. Reci korisniku što se dogodilo; ako je u sesiji dostupna ovlaštena veza s GitHubom, push napravi preko nje.
