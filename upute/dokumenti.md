# Rad s dokumentima

## Načela

- Dokumenti u ovom repozitoriju jedini su trajni zapis projekta. Što nije zapisano, za sljedeću instancu ne postoji.
- Svaki podatak ima jedno glavno mjesto. Drugi dokumenti na njega upućuju nazivom i poveznicom, ne kopiraju ga. Kad se podatak promijeni, promijeni ga ondje i provjeri dokumente koji ga spominju.
- `README.md` je kazalo. Svaki novi dokument mora biti dodan u njega, a svaki obrisani uklonjen.
- Ova pravila i mapa `upute/` ne sadrže projektne činjenice. Ne dodaji ih ovamo.

## Organizacija: opći dokumenti i dokumenti nekretnina

- **Opći dokumenti** (u korijenu repozitorija) sadrže ono što vrijedi za svaku nekretninu: pravila, parametre, formule, predloške i kontrolne liste.
- **Dokumenti nekretnina** (mapa `nekretnine/`) sadrže samo podatke, izračune i posebnosti jedne nekretnine. Pravila ne prepisuju, nego upućuju na opći dokument i u njega upisuju svoje ulazne podatke i rezultate.
- Nova nekretnina dobiva dokument napravljen iz predloška u mapi `nekretnine/` i red u pregledu nekretnina.
- Komunikacija se i dalje upisuje u dokument Kontakti i komunikacija; dokument nekretnine ima samo kratak tijek s uputom na njega.

## Kad nekretnina otkrije nešto novo

- Postavi pitanje: bi li to vrijedilo i za sljedeću nekretninu?
  - **Da:** upiši u odgovarajući opći dokument, a u dokumentu nekretnine ostavi samo primjenu i uputu.
  - **Ne:** ostaje u odjeljku Posebnosti te nekretnine.
  - **Nije jasno:** ostaje kod nekretnine s oznakom „možda opće”. Kad se ista stvar pojavi kod druge nekretnine, premjesti je u opći dokument.
- Kad nešto premjestiš u opći dokument, navedi to u odgovoru korisniku.

## Zastarijevanje

- **Parametri na jednom mjestu.** Primanja, vlastita sredstva, najveća rata i slični parametri žive samo u dokumentu Financijski okvir. Drugi dokumenti na njih upućuju.
- **Izračun bilježi s čime je napravljen.** Uz svaki izračun u dokumentu nekretnine navedi datum i parametre (npr. primanja, vlastita sredstva, kamatu). Kad se parametar u Financijskom okviru promijeni, preračunaj izračune aktivnih nekretnina koji ga koriste i reci to korisniku.
- **Promjenjive činjenice imaju datum.** Uz kamate, ponude, akcije, cijene radova, uvjete banaka i propise navedi izvor i „stanje na dan”. Okvirni rokovi zastarijevanja: kamate i ponude banaka oko mjesec dana, cjenici radova oko šest mjeseci, propisi do sljedeće izmjene.
- **Rokovi ponuda** (do kada vrijedi ponuda ili akcija) upisuju se u odjeljak Rokovi u dokumentu Proces kupnje kuće – koraci i dokumenti.
- **Arhiva se ne ažurira.** Kad nekretnina propadne ili je odbačena, premjesti njezin dokument u `nekretnine/arhiva/` (s `git mv`), na vrh upiši datum i razlog arhiviranja i promijeni status u pregledu nekretnina. Pouke koje vrijede općenito prenesi u opće dokumente.

## Kada stvoriti novi dokument

- Kad tema ima vlastitu svrhu i rast će s vremenom (npr. nova vrsta financiranja, nova nekretnina). Korisnik voli odvojene, međusobno povezane dokumente umjesto jednog velikog.
- Ponude banaka ne dobivaju zasebne dokumente; vode se u dokumentu Usporedba ponuda stambenih kredita, a detalji pojedine ponude kao njegov odjeljak.
- Prije stvaranja provjeri postoji li već dokument kojem tema pripada.

## Struktura dokumenta

- Naslov `#` je naziv dokumenta, a odmah ispod jedna do dvije rečenice sa zaključkom ili trenutnim stanjem.
- Odjeljci `##` s jasnim nazivima. Prva rečenica odjeljka je njegova poanta.
- Tablice za usporedbe, iznose i popise s više atributa. Kontrolne liste (`- [ ]` / `- [x]`) za korake i otvorena pitanja.
- Otvorena pitanja zapiši tamo gdje nastaju, kao kontrolnu listu. Riješena označi s `[x]` i kratkim odgovorom, ne briši ih.
- Na kraju odjeljak „Povezani dokumenti” i izvori kao poveznice. Poveznice među dokumentima pišu se kao relativne Markdown poveznice (dokumenti u `nekretnine/` upućuju na opće dokumente s `../`).
- Datume događaja u dnevnicima komunikacije piši od najnovijeg prema najstarijem.

## Ažuriranje

- Nakon svakog novog saznanja (odgovor banke, novi dokument, ispravak korisnika) ažuriraj sve dokumente na koje utječe, ne samo jedan.
- Zatvaranje otvorenih pitanja, upis komunikacije i rokova radi prema [tijek-razgovora.md](tijek-razgovora.md).
- Kad u odgovoru ili dokumentu objasniš pravni, bankarski ili građevinski pojam kojeg još nema u [pojmovniku](../Pojmovnik.md), dodaj ga ondje abecednim redom, s odgovarajućom temom.
- Kad korisnik ispravi sadržaj, prvo provjeri ispravak. Ako je točan, ispravi dokument. Ako nije, objasni zašto i ne mijenjaj.
- Ne briši korisnikove izmjene i komentare. Ako proturječe novim podacima, ukaži na to.
- Nakon izmjene napravi commit (vidi [git.md](git.md)).

## Datoteke

- Format je Markdown (`.md`) radi lakog pregledavanja na bilo kojem uređaju i praćenja promjena kroz git.
- Binarne datoteke (Word, Excel, PDF) ne drže se u repozitoriju osim ako korisnik to izričito traži. Izračune zapiši kao Markdown tablice s opisom formule.
- Izvorne dokumente koje korisnik dostavi (ponude, dozvole, elaborate) analiziraj, ali ih ne dodaji u repozitorij bez dopuštenja, jer mogu sadržavati osobne podatke.
