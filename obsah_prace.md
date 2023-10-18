# Obsah Práce

1. Úvod
   1. Čo je PLONK
   2. Prečo je dôležitý
   3. Pre koho je vhodný tento článok
2. Background
    1. Zero-Knowledge
    2. SNARKy
    3. Využitie v praxi
3. Vysvetlenie PLONKu
   1. Zjednodušené vysvetlenie konceptu
   2. Detailne vysvetlenie jednotlivých komponentov
   3. Spájanie komponentov
   4. Výhody & Limitácie
4. Porovnania
   1. PLONK oproti ostatným ZK-SNARKom
   2. Rôzne implementácie PLONKu
5. Zhrnutie optimalizácií PLONKu
   1. Popis poznaných optimalizácií
   2. Implementácia optimalizácia v kóde
6. Výsledky benchmarkov
   1. Grafy a tabuľky
   2. Popísanie výsledkov

## Zameranie (Konwledge Gap)

Šifrovací systém je dôkladne popísaný, avšak prekúsať sa cez článok je náročné. Ostatné zdroje blogy a videá sú buď o úplných základoch proof systému alebo už vysvetľujú PLONK pre ľudí ktorý mu rozumejú. Tento článok by mal vyplniť túto medzeru a dôkladne vysvetliť ako systém funguje, ľuďom ktorí už majú znalosti z matematiky ale nestretli sa so ZK. Okrem toho bude obsahovať aj **porovnanie s inými ZK-SNARKami a zhrnutie poznaných optimalizácií**, ktoré som doposiaľ nenašiel voľne dostupné.

## Vysvetlenie PLONKu

Veľa blogov ktoré sa snažia PLONK vysvetliť pracovali s nejakým konkrétnym príkladom. To je z hľadiska práce moc neformálne. Postup vysvetlenia ktorý funguje najlepšie pre mňa je:

1. Zjednodušené vysvetlenie konceptu
    1. Ako spolu komponenty proof systému spolupracujú
    2. Uvedenie high-level diagramu
    3. (príklad na ktorom by sa to dalo ukázať)
2. Detailne vysvetlenie jednotlivých komponentov
    1. Každý z nich bude mať krátky popis ktorý bude rozšírením zo zjednodušeného vysvetlenia v úvode
    2. Formálne vysvetlenie s definíciami atď.
    3. Dokázanie požadovaných matematických vlastností (veľa zdorov to odfláklo:)
3. Spájanie komponentov
    1. Presné vysvetlenie integrovania komponentov
    2. Detailný diagram
    3. (rozšírenie príkladu z úvodu)

Výhody tohto prístupu sú:

1. V každej časti článku čitateľ vie čo sa snažím vysvetliť aká je motivácia a kde jednotlivé časti zapadajú. V niektorých článok som sa často strácal s tým, že som nevedel čo je cieľom danej časti.
2. Prehľadnosť práce, jednoduché hľadanie informácií
