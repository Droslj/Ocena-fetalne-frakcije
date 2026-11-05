# Ocena-fetalne-frakcije
Ocena fetalne frakcije v prostoležeči DNA (cffDNA)

**Povzetek (Abstract / Executive Summary)**
Oceniti delež fetalne frakcije (FF) in število veljavnih informativnih markerjev iz vzorcev prostoležeče DNK (ccfDNA) v materini plazmi ter ovrednotiti zanesljivost rezultatov za klinično ali raziskovalno poročilo. Pri delu sem uporabil podatke iz sledečega projekta [1].

**Pristop**
Združevanje in obdelava genomskih podatkov za posamezne indele (alela A in B), filtriranje podatkov glede na stroge biološke kriterije ter hkratna vizualizacija vrednosti in statistične zanesljivosti.

**Ozadje in biološko-metodološko ozadje**

Metodologija izračuna:
Fetalna frakcija se za posamezni indel izračuna z upoštevanjem diploidne narave ploda (faktor 2) in razmerja med fetalnim alelom ter skupno pokritostjo

:$$\text{FF} = 2 \times \left( \frac{\text{fetalni alel}}{\text{skupna pokritost}} \right) \times 100\,\%$$

Izračun se lahko izvede neposredno z množenjem obstoječega deleža mutiranega alela z 200.

Kriterij informativnosti: 
V analizi so bili kot veljavni (informativni) upoštevani le tisti markerji, katerih vrednost fetalne frakcije pade v biološko smiselen in zanesljiv razpon med 1,5 % in 50 %, s čimer se izločijo šumi in tehnične napake.

Potek dela in implementacija v ExceluAvtomatizacija izračunov: Uporaba naprednih Excelovih funkcij za obdelavo podatkov po celotni matriki vzorcev.Filtriranje in povprečenje: Uporaba funkcije AVERAGEIFS za izračun končne povprečne fetalne frakcije z izločitvijo vrednosti izven predpisanega območja.Ovrednotenje zanesljivosti ($N$): Uporaba funkcije COUNTIFS za število veljavnih informativnih markerjev na posamezen vzorec. S tem je bil uveden ključen indikator kakovosti, saj se vzorci razlikujejo v številu zanesljivih meritev (od posameznih markerjev do bogatejših naborov 4–5 markerjev).4. Rezultati in vizualizacijaAnaliza vzorcev: 

Obdelanih je bilo 15 ustreznih vzorcev (ob predhodnem izločanju neustreznih v zgornjem delu cevovoda). Končne vrednosti fetalne frakcije se smiselno gibljejo v pričakovanih bioloških okvirih.

Grafični prikaz: Izdelan je bil kombiniran stolpčni grafikon, ki hkrati in pregledno prikazuje:Delež fetalne frakcije (ločeno za alela A in B, prikazano modro).Število veljavnih informativnih markerjev (prikazano rdeče), ki služi kot vizualni pokazatelj statistične robustnosti posameznega rezultata.

5. Zaključek in priporočila
6. Pristop omogoča hitro, pregledno in zanesljivo kvantifikacijo fetalne frakcije iz ccfDNA podatkov.
7. Poudarjena je nujnost hkratnega spremljanja števila informativnih markerjev, saj rezultati, ki temeljijo na zelo majhnem številu točk (npr. 1 marker), zahtevajo večjo previdnost pri interpretaciji.
 


**Reference**
[1] Cell-free DNA sequencing using insertion/deletion polymorphisms, 
    Project PRJNA387652 (https://www.ncbi.nlm.nih.gov/bioproject/PRJNA387652)
