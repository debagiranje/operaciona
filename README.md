# operaciona
projekat iz predmeta operaciona istrazivanja na temu "The minimum quasi clique partitioning problem"

# TODO
[ ] pronaci instance razlicitih velicina (mozda cak pitati autora rada da nam posalje svoje, da mozemo uporediti rezultate(?))
[ ] pokusati pronaci jos neki rad za referisati se
[ ] Greedy -- nakon implementacije algoritma, napraviti skripticu koja ce nam ga pustati 1x po instanci grafa. (Mozda da dumpamo rezultate u txt file?) -- po uputstvima svakako...
    -- note, trebalo bi svakako napraviti skriptu za hvatanje rezultata "pustanja" algoritama nad svim instancama, necemo pojedinacno...
[ ] VNS -- ...
[ ] CPLEX (PuLP biblioteka) -- ...
[ ] napraviti okrvir dokumentacije u lateku (mislim da sam nekad nekakav sklepala)

notenote: dodaj svoj inicijal kraj stavke koju zelis da odradis, da se raspodijelimo


# uputstva 
Dokumentacija projekta treba da sadrži sljedeće komponente za problem koji ste odabrali za rješavanje:

1) Definiciju prostora pretrage, funkcije cilja, funkcija prilagodljivosti (po mogućnosti), komponentu rješenja.

2) Pohlepni pristup rješavanju problema gdje treba definisati  pohlepnu funkciju, dodavanje komponente u rješenje.

3) Genetski ili VNS pristup (odaberite jedan od ova dva algoritma po želji)
     - Za genentski: definisati jedinku, operator selekcije, ukrštanja, operator mutacije.
     - Za VNS: definisati lokalnu pretragu, strukture okolina, objasniti zašto su baš takve uzete.

4) Implementirati model u CPLEX-u (ili PuLp, ako se odlučite za jezik python za implementiranje).

Poređenje rezultata:

1) Prvo nađite instance za vaš problem. Ako postoje problemi u nalaženju istih, javite se meni pa ćemo zajedno da ih potražimo.
2) Odaberite maksimalno 50 instanci (30 je neki okvirni broj) na kojima ćete da testirate vaše algoritme. Neka budu raznovrsne po svojoj dimenziji (dakle, nekoliko  malih instanci, zatim nekoliko srednjih i  nekoliko velikih).
3) Pohlepni algoritam puštate samo jednom po instanci. Bilježite  vrijednost rezultata i vrijeme potrebno da se ovaj pristup izvrši. 
Genetski/VNS pristup puštate min 5 ili idealno 10 puta na jednoj instanci. Bilježite srednju vrijednost rezultata (za 10 puštanja date instance), maksimalnu  vrijednost (u 10 puštanja), standardnu devijaciju rezultata i srednju  vrijednost izvršavanja (na 10 puštanja). CPLEX puštate jednom po  instanci gdje bilježite rezultat koji je vraćen i vrijeme izvršavanja.  Sve ovo prikažite u jednoj (ili više) tabela -- možete recimo imati 3 tabele, jednu za rezultate na malim instancama, jednu tabelu za  rezultate na srednjim instancama i jednu za rezultate za velike instance. najbolji rezultat za svaku instancu među ova tri algoritma  boldovati radi preglednosti.
4) Prodiskutovati rezultate: na koliko instanci jedan algoritam daje bolja rješenja, na koliko drugi, itd.  Brzinu izvršavanja algoritma, koliko je instanci XPLEX riješio do optimalnosti itd.
5) Vrijeme za svaki od algoritama ograničiti na (maksimalno) 10 minuta. 
