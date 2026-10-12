# Rad s dokumentima

## Načela

- Dokumenti u ovom repozitoriju jedini su trajni zapis projekta. Što nije zapisano, za sljedeću instancu ne postoji.
- Svaki podatak ima jedno glavno mjesto. Drugi dokumenti na njega upućuju nazivom i poveznicom, ne kopiraju ga. Kad se podatak promijeni, promijeni ga ondje i provjeri dokumente koji ga spominju.
- `README.md` je kazalo. Svaki novi dokument mora biti dodan u njega, a svaki obrisani uklonjen.
- Ova pravila i mapa `upute/` ne sadrže projektne činjenice. Ne dodaji ih ovamo.

## Kada stvoriti novi dokument

- Kad tema ima vlastitu svrhu i rast će s vremenom (npr. nova ponuda, nova vrsta dokumentacije). Korisnik voli odvojene, međusobno povezane dokumente umjesto jednog velikog.
- Prije stvaranja provjeri postoji li već dokument kojem tema pripada.

## Struktura dokumenta

- Naslov `#` je naziv dokumenta, a odmah ispod jedna do dvije rečenice sa zaključkom ili trenutnim stanjem.
- Odjeljci `##` s jasnim nazivima. Prva rečenica odjeljka je njegova poanta.
- Tablice za usporedbe, iznose i popise s više atributa. Kontrolne liste (`- [ ]` / `- [x]`) za korake i otvorena pitanja.
- Otvorena pitanja zapiši tamo gdje nastaju, kao kontrolnu listu. Riješena označi s `[x]` i kratkim odgovorom, ne briši ih.
- Na kraju odjeljak „Povezani dokumenti” i izvori kao poveznice.
- Datume događaja u dnevnicima komunikacije piši od najnovijeg prema najstarijem.

## Ažuriranje

- Nakon svakog novog saznanja (odgovor banke, novi dokument, ispravak korisnika) ažuriraj sve dokumente na koje utječe, ne samo jedan.
- Zatvaranje otvorenih pitanja, upis komunikacije i rokova radi prema [tijek-razgovora.md](tijek-razgovora.md).
- Kad korisnik ispravi sadržaj, prvo provjeri ispravak. Ako je točan, ispravi dokument. Ako nije, objasni zašto i ne mijenjaj.
- Ne briši korisnikove izmjene i komentare. Ako proturječe novim podacima, ukaži na to.
- Nakon izmjene napravi commit (vidi [git.md](git.md)).

## Datoteke

- Format je Markdown (`.md`) radi lakog pregledavanja na bilo kojem uređaju i praćenja promjena kroz git.
- Binarne datoteke (Word, Excel, PDF) ne drže se u repozitoriju osim ako korisnik to izričito traži. Izračune zapiši kao Markdown tablice s opisom formule.
- Izvorne dokumente koje korisnik dostavi (ponude, dozvole, elaborate) analiziraj, ali ih ne dodaji u repozitorij bez dopuštenja, jer mogu sadržavati osobne podatke.
