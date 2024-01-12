Projekt z MPS - 2D hra - Hartman

Dobrý den posílám lépe vysvětlený projekt z MPS. Účelem projektu je vytvořit plně funkční 2D hru na PC která bude obsahovat plně funkční animace, objekty a pohyby hráče.
S programováním her mám už menší zkušenost, protože už jsem si jednu hru zkoušel programovat, ale bohužel jsem jí nedokočil a díky tomu jsem se rozhodl právě pro tento typ projektu.

Hru jsem tvořil v Unity a programoval ve Visual Studio Code, protože s tímto programem mám již zkušenosti ze školy.
Jak již jsem dříve psal inspiraci jsem si vzal z této série videí: https://youtu.be/TcranVQUQ5U?list=PLgOEwFbvGm5o8hayFB6skAfa8Z-mw4dPV a všechny použité herní textury jsem si stáhnul právě z tohoto videa.

Po založení nového projektu v Unity jsem si zhlédnul výše uvedenou sérii videí a snažil se toho co nejvíce pochytit, abych do budoucna mohl postupovat samostatně. 

Hned po založení projektu jsem si založil nový objekt s názvem Player, základní scénu jsem pojmenoval Levels a založil tři nové jménem Scripts, Sprites a Animations. (většinu jsem záměrně pojmenoval Anglicky, aby jsem se mohl v případě nejistoty kouknout na video a postupovat podle něho.)
Následně jsem do scén přetáhnul všechny soubory a objekty které byly potřeba.

![Výstřižek](https://github.com/hartmanjan1/Projekt-/assets/156115281/e3511117-7e10-40e9-896a-99c0bba4fb89)

Pokračoval jsem tak že jsem si založil nový objekt s názvem Level 1 a přidával herní textury tak aby level vypadal co nejlépe. Základem byla "podlaha" která musela plnit takovou funkci aby se na ní hráč udržel a nepropadnul dolů, to jsem zapříčinil tak že jsem na každou  
část podlahy přidal schopnost Box Collider 2D to znamená že hráč už mohl na podlahu stoupnout a nepropadl se. Tuto funkci jsem dal na všechny textury na které hráč v daném levelu stoupne.

![Výstřižek2](https://github.com/hartmanjan1/Projekt-/assets/156115281/b16f284a-afa1-43d0-abb5-7eea74a26153)

Dále jsem pokračoval tím že jsem se přesunul na objekt jménem Player. Na tento objekt jsem také přidal Box Collider 2D ale musel jsem přidat ještě Rigidbody 2D což způsobí to že objekt bude mít "fyzické tělo" a ovlivní to jeho gravitaci. Na objekt jsem pak přidal texturu draka aby to vypadalo lépe.

![Výstřižek3](https://github.com/hartmanjan1/Projekt-/assets/156115281/f54bf0ee-1e16-46a3-a35f-0a9b851af4a5)

Pak jsem ve složce Scripts založil nový C# Script díky kterému jsem se přesunul do Visual Studia a mohl začít psát první kódy. Přiznám se že jsem ze začátku nevěděl jaké kódy budou potřeba, proto jsem se znovu podíval na video a snažil se pochopit jak jednotlivé kódy fungují a k čemu jsou potřeba.

Začal jsem tímto příkazem: 

![Výstřižek 4](https://github.com/hartmanjan1/Projekt-/assets/156115281/002eb0df-f821-4083-9efe-e4c1ce5793c7)

Který mi pomohl v tom aby se tělo hráče pohybovalo. Hráč se už sice pohyboval, ale velmi malou rychlostí takže jsem přidal další řádek příkazu který rychlost opravil. Rychlost jsem si mohl nastavit přímo v Unity v Player Movement Script - Speed kde jsem nastavil rychlost 10.

![Výstřižek 5](https://github.com/hartmanjan1/Projekt-/assets/156115281/bffe292a-63fe-462c-93b8-ed154086615e)
![Výstřižek 6](https://github.com/hartmanjan1/Projekt-/assets/156115281/fc709eee-b983-4d2f-8b74-bb23e9e425a0)

Jelikož se hráč už poměrně dobře pohyboval bylo na čase přidat skok který jsem přidal jednoduchým příkazem:

![Výstřižek 7](https://github.com/hartmanjan1/Projekt-/assets/156115281/0e6e8a22-b55a-4810-9840-b4a6e282b235)



