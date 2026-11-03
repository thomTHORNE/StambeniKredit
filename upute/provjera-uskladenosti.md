# Provjera usklađenosti dokumenata

Povremeni pregled cijelog repozitorija: traže se duplikati, proturječja, zastarjeli podaci i podaci na krivom mjestu. Provjera pokreće se na zahtjev korisnika ili kao zakazani zadatak. Ne mijenja dokumente sama: rezultat je izvještaj, a izmjene se rade tek kad ih korisnik odobri.

## Postupak

1. Dohvati repozitorij i radnu granu prema [git.md](git.md). Pročitaj `CLAUDE.md`, sve upute i sve dokumente iz `README.md`, uključujući mapu `nekretnine/` (arhivu samo radi provjere poveznica i prenesenih pouka).
2. Provjeri svaku od kategorija niže i zapiši nalaze.
3. Izvještaj pošalji korisniku. Za svaki nalaz navedi dokument i odjeljak, što je problem i prijedlog rješenja.
4. Ništa ne mijenjaj bez odobrenja. Iznimka su očite tehničke greške (pokvarena poveznica, krivi naziv dokumenta u poveznici); njih ispravi, napravi commit i navedi ih u izvještaju.

## Što se provjerava

| Kategorija | Što tražiti |
| --- | --- |
| Duplikati | Isti podatak zapisan na više mjesta, i drugim riječima. Prema pravilu jednog mjesta ostaje samo u glavnom dokumentu, ostali upućuju na njega. |
| Proturječja | Različiti iznosi, datumi, imena ili statusi istog podatka u različitim dokumentima. |
| Zastarjelo | Promjenjive činjenice čiji je „stanje na dan” stariji od okvirnog roka iz [dokumenti.md](dokumenti.md); rokovi u odjeljku Rokovi koji su prošli ili ističu u sljedećih 14 dana; izračuni aktivnih nekretnina napravljeni sa starim parametrima iz Financijskog okvira. |
| Krivo mjesto | Opća pravila zapisana u dokumentu nekretnine (ili stavke označene „možda opće” koje se pojavljuju kod više nekretnina) i podaci jedne nekretnine u općim dokumentima. |
| Otvoreno | Stavke „Pripremljeno” u Kontaktima starije od tjedan dana; otvorena pitanja (`- [ ]`) bez napretka; oznake „pretpostavka – potvrditi”. |
| Struktura | Pokvarene relativne poveznice; dokumenti kojih nema u `README.md`; pojmovi objašnjeni u dokumentima, a kojih nema u Pojmovniku. |

## Oblik izvještaja

- Prva rečenica: koliko je nalaza i koji je najvažniji.
- Nalazi grupirani po kategorijama, najvažniji prvi; za svaki dokument, odjeljak, problem i prijedlog.
- Na kraju popis eventualno ispravljenih tehničkih grešaka i commit.
- Ako nema nalaza, to jasno reći u jednoj rečenici.
