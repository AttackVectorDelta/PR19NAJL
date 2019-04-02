# Analiza osebnih avtomobilov v Sloveniji

## Seznam članov:
* Nejc Ačkun
* Jernej Leskovšek


## Podatki in predprocesiranje
Odločila sva se, da bova kot najino zbirko podatkov uporabila evidenco vseh registriranih vozil v Sloveniji. Podatke se lahko najde tukaj: https://podatki.gov.si/dataset/evidenca-registriranih-vozil-presek-stanja.

Zbirka je sestavljena iz približno 2 miljona elementov. Mislila sva, da je zbirka že omejena na avtomobile, ampak zbirka vsebuje VSA vozila v Sloveniji, in vključuje:
 * Motorna kolesa
 * Delovne stroje
 * Dvigala
 * Traktorje
 * Priklopnike itd.
 
Odločila sva se, da se bova omejila samo na avtomobile. Oba naju zanimajo avtomobili, in sklepava, da bova tako lahko tudi lažje potrdila dobljene rezultate oz. lažje opazila napake in posebnosti, ki bi se lahko pojavile. 

Na srečo v podakovni zbirki obstaja stolpec, ki opisuje tip vozila, tako da je bila filtracija trivialna.

Po filtraciji sva naletela še na kar nekaj problemov. Obstaja več atributov, ki se navezujejo samo na določen tip vozila (recimo stolpec "Q-Razmerje moc/masa (samo za motorna kolesa)"). Te stolpce sva pobrisala pred začetkom analiz.

Drugi večji problem pa so nekonsistentnosti pri podatkih. Lep primer tega je recimo proizvajalec "Alfa Romeo". V podatkih se pojavijo kar trije različni načini zapisa (ALFA ROMEO, ALFA-ROMEO, ALFA- ROMEO). Te podatke sva seveda popravila, ampak samo zato, ker točno veva pravilno obliko podatkov. 

Zaplete se recimo pri stolpcu "D.3-Komerc. oznaka" kjer so podatki model, prostornina motorja in še kakšna druga lastnost ločeni z znakom "/". Tukaj pa pravilnosti, oz. večih vnosov z istim pomenom ne moreva več zaznavati in popravljati.


