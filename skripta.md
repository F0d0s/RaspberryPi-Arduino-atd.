# Arduino, Raspberry Pi, atd.
## Úvod
Jak vypovídá název, budu Vám chtít něco říct o Arduinu, Raspberry Pi a dalších podobných věcech. Avšak na začátek bych chtěl upozornit na jednu věc.  

Co to vlastně je zač. Arduino a Raspberry Pi se dají považovat za **jednodeskové počítače**. Když se ale kohokoliv na ulici ale zeptáte co je to počítač tak vám začne popisovat normální stolní počítač nebo notebook. To by ještě z části odpovídalo Raspberry Pi, u kterého na všechny modely kromě jednoho jde nainstalovat operační systém a vážně s ním zácházet jako s  „normálním" počítačem. Arduino však ne. U tohoto je dle mého názoru lepší ho nazvat vývojovou deskou. No a jaký je mezi tím rozdíl?  

### Jednodeskový počítač
Jedna deska plošných spojů, která na sobě má všechny potřebné komponenty a bohaté možnosti rozšíření o další hardware (I/O moduly atd.)  

### Vývojové desky
Univerzální platformy, umožňující vytvoření mikrokontrolerové aplikace během velice krátkého času a za velice dostupné ceny, hlavní částí jsou různé doplňující komponenty, bez nich jsou prakticky k ničemu.  

*První definice se dá pojat i trochu jinak aby odpovídala oboum, avšak pro účely těchto skript a prezentace bych to chtěl takto rozdělit, aby tyto pojmy byli více přehledné a celkově aby to dávalo větší smysl, protože Raspberry Pi a Arduino není to stejné.*  

Na co vše se ale dají takovéto věci používat? Všude na internetu najdete spoustu nápadů využití, tyto všechny se ale určitě dají rozdělit do různých skupin.  
* IoT - různá IoT zařízení, od čidel, po chytré vymoženosti.
* Projekty - jakékoliv kreativní projekty, roboti atd.
* Výuka - výuka programování a zapojování ve školách.  

Toto samozřejmě není vše ale do těchto tří spadá nejvíce využití.

## Raspberry Pi
Raspberry Pi jsou ve většině případů jednodeskové počítače. Pochází z Velké Británie originálně vytvořené od **Raspberry Pi Foundation**.  

Prvního Raspberry Pi jsme se dočkali roku **2012 (Raspberry Pi Model B)**, ke kterému se dostaneme ještě později. Tento model odstartoval tuto celou řadu počítačů a zároveň tento celkový trend jednodeskových počítačů.  

Raspberry Pi jsou vytvářeny ve spolupráci s firmou **Broadcom**, která dodává **SoC (System on chip)** do prakticky všech Raspberry Pi. Tyto čipy mají v sobě vše potřebného k provozu těchto jednodeskových počítačů od procesoru až po RAM.  

Jakožto skoro právoplatné počítače mají samozřejmě operační systém. Je zde mnoho možností od oficiálního **Raspberry Pi OS** až po různé další distribuce Linuxu, včetně i více zaměřených jako LibreELEC, což je distribuce přímo určená k fungování jako takzvané „media centre". Na novějších modelech se dokonce dá rozběhnout i Windows 10.  

### Raspberry Pi Model B
Tento model je již zmiňovaný úplně první prodávaný jednodeskový počítač Raspberry Pi vydaný v roce 2012. V celé této generaci však bylo více modelů, které byly o něco lepší než ten předešlí, nebo měly jinou velikost a byly o něco jednodušší. Většinou se ale jednalo o vylepšení procesoru a dalších komponentů.  

**Procesor:** ARM1176JZF-S, 700MHz  
**RAM:** 512 MB  

Samozřejmě nechybí **GPIO**, kterého na tomto modelu ale není tolik jako na dnešních modelech, na tomto je **8x**. Nechybí také vývod na napájení 3.3 V a 5 V. Jakožto u každého Raspberry Pi tak se zde nachází i RJ45 a oproti novějším modelům jenom **2x USB**. K připojení k monitoru je k dispozici HDMI. Nachází se zde také RCA a 3.5 mm Jack.  

### Raspberry Pi 2
Jakožto s každou další generací zde přichází vylepšení procesoru a RAM. Avšak procesor není jenom rychlejší ale v pozdější verzi 1.2 je vylepšen i na 64-bitovou architekturu. Byl vydaný v roce 2015.  

**Procesor:** 64-bitový  ARM Cortex-A53, 900 Mhz (verze 1.2, předešlá měla 32-bitový ARM Cortex-A7)  
**RAM:** 1 GB  

Zde se již nachází standartních 4x USB portů. Avšak přicházíme o RCA z minulé generace *(RCA = druh konektoru, přes který se přenáší audio a video)* Oproti předešle zmíněném modelu zde konečně máme více GPIO pinů, přesněji 40.  

### Raspberry Pi 3
U této generace z roku 2016 jak bude všude zvykem máme zase vylepšený procesor, který dosahuje rychlosti 1.2 GHz. Avšak se jedná o stejný procesor, protože předešlá generace ho měla podtaktovaný.  

**Procesor:** 64-bitový  ARM Cortex-A53, 1.2 GHz  
**RAM:** 1 GB  

Novinkou jsou zde možnosti bezdrátového připojení jak **WiFi** tak i **Bluetooth**. Dále přibývá i možnost bootování z USB.  

### Raspberry Pi 4
Dostáváme se již k skoro nejnovějšímu modelu Raspberry Pi, tento vyšel roku 2019. Mezi Raspberry Pi 3 a 4 není velká mezera, jenom mezi tím vycházely vylepšené verze Raspberry Pi 3. Nesmí samozřejmě chybět vylepšený procesor a konečně nám tato generace přináší i možnost si vybrat kolik RAM chceme.  

**Procesor:** 64-bitový ARM Cortex-A72, 1.5 GHz  
**RAM:** 1, 2, 4, 8 GB (na výběr)  

U tohot modelu máme vylepšené skoro vše. Ethernet je konečně neomezený, máme zde lepší WiFi, Bluetooth 5 a spoustu dalšího. Novinkou jsou taky 2x 4K micro HDMI porty a 2x USB 3.0 porty.  

### Raspberry Pi 5
Toto je nejnovější přispěvek do Raspberry Pi rodiny, který byl vydán již minulý rok, 2023. Je skoro dvakrát rychlejší než předešlá generace a otevírá mnoho dalších možností s pomocí dalších vylepšení. Zde máme už na výběr jenom z dvou RAM možností.  

**Procesor:** 64-bitový Arm Cortex-A76, 2.4 GHz  
**RAM:** 4, 8 GB  

Tento model je první, který využívá I/O čip přímo od Raspberry Pi, RP1. Toto umožňuje rychlejší komunikaci prakticky všeho, tento čip stojí mezi SoC a všemi I/O. Novinkou je taky RTC čip (Real-Time Clock), který se stará o čas. Další je možnost připojení pomocí PCI express, což umožňuje například připojit M.2 SSD k tomuto malému počítači a umožnit mu rychlejší přenosy atd. Bohužel jsme se ale museli rozloučit s 3.5 mm Jack :(  

### Raspberry Pi Zero
Tento model není pokračování v předešlé sérii. Je to sám o sobě jiný produkt. Jedná se o kompaktnější stále jednodeskový počítač. *(může se na něj nainstalovat OS, jako napříkald Raspberry Pi OS)*  

**Procesor:** 64-bitový Arm Cortex-A53, 1 GHz  
**RAM:** 512 MB  

Nachází se zde RP3A0, což je SiP (System in Package) vytvořené samotným Raspberry Pi. Skladá se ze stejného čipu, který byl použit v Raspberry Pi 3. Nechybí bezdrátové připojení WiFi a Bluetooth. Avšak chybí Ethernet a USB porty kvůli kompaktnosti.  

### Raspberry Pi Pico
Zde se podle mých definicí již jedná spíše o vývojovou desku. Je zde zase čip přímo od Raspberry Pi akorát je to RP2040. Tato deska je programovatelná pomocí Micro Pythonu a popřípadě i C/C++. Nachází se na ní pouze GPIO, 3 piny/porty na debugování a jedno micro USB pro napájení.  

**Procesor:** ARM Cortex-M0+, 133 MHz  
**RAM:** 264 kB  

### Využití Raspberry Pi
Raspberry Pi jendodeskové počítače se dají využít na mnoho věcí. Asi nejvíc nečekané využití je prostě jako stolní počítač. Někteří prostě nepotřebují výkon a chtějí třeba jenom brouzdat po internetu.  

Jenže tento počítač doho dokáže o dost více. Můžete ho použít prakticky jako skoro jakýkoliv server. Od print serveru (server, který se stará o bezdrátové tisknutí v tiskárně), kterým můžete proměnit svoji drátovou tiskárnu na bezdrátovou či růtzné IoT servery atd. Využití je spousta.  

Další využití, o kterém jste nejspíš slyšeli je takzvané „media centre", jde o to že Raspberry Pi dokáže přehrávat jakýkoliv obsah v celkem dobré kvalitě a tak spolu s jeho skladností je ideální na připojení k televizi, nebo čemukoliv jinému a přehrávání například Netflixu, Kodi atd. Další využití je takové spíše pro zábavu a to je emulace retro videoher. K tomuto využití je dokonce vyvýjen i software, takže v této době už jednoduché si něco takového vytvořit.  

U nás doma se tyto jednodeskové počítače využívají na více věcí ale nejhlavnější jsou asi 3D tiskárny, na kterých obou běží Klipper a tak se nám Raspberry Pi stará nejen o vzdálený přístup, ale i vylepšené a celkově přesnější a rychlejší tisky.  

No a pokud byste už vůbec nevěděli co se svým Raspberry Pi dělat, můžete na něm těžit něco jako DUINOCoin nebo dokonce i Monero ;)  

## Arduino
Arduino jsou vývojové desky původem z Itálie. Tento open-source projekt založili Massimo Banzi, David Cuartielles, Tom Igoe a David Mellis. Údajně vznikl tak, že rozšířili projekt Wiring od Hernando Barragána o podporu levnějšího mikrokontroléru ATmega8.  

Jak už jsem to nakousl, Arduino využívá mikrokontroléry ATmega.  (8-bitové) Později se dostali i do 32-bitového světa s deskou Arduino Due, ale to už nebyl ATmega, ale AT91SAM3X8E (ARM procesor).  

K těmto vývojovým deskám začali vyvýjet i vývojové prostředí Arduino IDE, které se používá do teď a je stále aktualizované. Je založeno na jazycích C/C++, takže se to tomu hodně podobá, ale je rozšířeno o různé knihovny, které ulehčují práci.

### Arduino desky
Zde na tomto obrázku můžete vidět, shrnutí prakticky celé historie Arduina, kde začínalo až po rok 2017. Do dneška samozřemě stále vychází nové modely a jsou čím dál tím lepší a lepší.  

![Alt text](https://cdn.discordapp.com/attachments/1098263330684162202/1193537630420353094/1704037402617-ef2c9441-5927-4649-a0d8-d0d93bebcfd5_1.jpg?ex=65ad1389&is=659a9e89&hm=dc6261c1e9d59a2a5766493c8bf0dabc6ab0169123ed4b42ad26673f3c4e343c&)  

### Využití Arduina
Oproti Raspberry Pi se jedná o vývojové desky, takže se s nimi spíše dělají různé projekty jako například roboti, čidla atd. Avšak možnosti jsou skoro nekonečné. Na internetu najdete spoustu ať už užitečných nebo jenom jednoduchých projektů.  

Samozřejmě, využívají se taky hodně ve výuce, jak programování tak i celkově elektroniky. Různá čidla a doplňující komponenty jsou prakticky hlavní částí Arduina a ty jsou určitě také zajímavá.  

Já sám moc arduina už nepoužívám, i když jsem chtěl založit můj projekt k tomuto tématu na jedné z desek Arduino, ale kvůli více možnostem už i například můj otec přechází na desky s čipy ESP, o kterých se vzápětí dozvíte.  

## ESP32 a ESP8266
Jedná se o čipi, které se používají na prakticky stejnojmenných vývojových deskách. Avšak ne těch se vyskytují z většiny ve formě modulů. Samozřejmě existuje také několika verzí těchto čipů ale základem je to že to jsou SoC čipy, které v sobě mají zabudované i bezdratové připojení WiFi a v případě ESP32 i Bluetooth.  

### ESP32
**Procesor:** Tensilica Xtensa 32-bit LX6, 240 MHz  
**RAM:** 520 kB  

Má jak WiFi tak i Bluetooth a náchází se na něm 34 GPIO. Setkáte se s ním v podobě modulu, například WROOM-32.

### ESP8266
**Procesor:** Tensilica L106 32-bit, 160 MHz  
**RAM:** 160 kB  

Má pouze WiFi a náchází se na něm 17 GPIO. Setkáte se s ním v podobě modulu, například WROOM-02.

### Vývojové desky
Jak jsem říkal, ESP32 a ESP8266 jsou čipy a ty se vyskytují ve formě modulů na vývojových deskách. Tyto moduly jsou tak předpřipravené, aby je prakticky stačilo jenom napájet na danou desku. Tyto vývojové desky výrábí různí výrobci ale výsledek je většinou stejný. I samotné Espressif vyrábí svou desku.  

V tuto dobu ale dokonce i Arduino pochitilo to, že ESP vývojové desky jsou docela žádané v této době, a tak vyšli například s produktem Arduino Nano ESP32, který má již zmíněný čip rovnou na sobě.  

### Využití
ESP čipy a i vývojové desky mají hlavní využití v IoT, nejen kvůli svým funkcím, ale i velikosti. Například jsem jeden našel ve své staré chytré zásuvce, která bohužel přestala fungovat :( Dají se s nimi i například vytvářet různá čidla které rovnou bezdrátově komunikují atd.

Avšak samozřejmě se dají využít při různých projektech, viz můj projekt. Celkově se jedná o výkonnější a více využitelnější Arduino, dokonce se dají programovat i pomocí stejného softwaru, Arduino IDE.  

Co se týče mého příkladu, tak u nás má otec zřízená čidla na chalupě, přes které monitoruje teplotu, tlak, vlhkost a CO2 v různých pokojích. Toto vám nejspíš ukáži v příkladech.  

## Srovnání
Dostáváme se k finálnímu srovnání, které slouží jako i takové spíše shrnutí. Začneme od začátku.  

**Raspberry Pi** - Jsou to jednodeskové počítače, které se dají prakticky nahradit za  „normální počítač". Běží na nich nějaký OS, který může mít jakékoliv rozhraní. Je u nich možnost připojit se k displeje. Prostě je o dost výkonnější a celkově má i lepší I/O možnosti.  

**Arduino** - Vývojové desky, které jsou závislé na tom jaké vedlejší komponenty k nim připojíte. Nedokážou se chovat jako „normální počítač". Dají se programovat, vytvoříte program a ten na nich do nekonečna běží. Jsou kompaktní a dají se využít skoro u každého projektu.  

**ESP** - V uvozovkách vylepšené verze Arduina. Jsou výkonnější a mají bezdrátové možnosti. Dají se programovat se ve stejném prostředí jako Arduino. Využívají se kvůli svým vlastnostem hodně v IoT.  

## Ostatní
Samozřejmě jako u každého produktu, i Raspberry Pi má své oponenty. Ti se snaží buď úplně zkopírovat samotný výrobek, nebo vytvořit lepší, menší či jinak vynikající produkt. Za zmínku stojí například Rock Pi, které nabízí Rock Pi S, s menšími rozměry než normální Raspberry Pi.  

Další zmínkou by mohli být také Banana Pi a Orange Pi. Banana Pi nabízí mimo jiné i routery. Orange Pi zase nabízí bohatou nabídku různých vývojových desek a jednodeskových počítačů, různé velikosti funkce, o dost více než Raspberry Pi.  

Tyto všechny počítače využívají však jiné SoC. Většinou jsou to jsou čipy Rockchip, nebo Allwinner.  

Arduino se také nevyhlo „klonům" a konkurentům. Existují také desky, které se buď úplně přesně snaží napodobit Arduino nebo také jenom prostě nabídnout třeba levnější verzi podobné desky.

## Ukázky
### Hlavní projekt - FPV Laptimer
Jedná se o vývojovou desku ESP32, ke které je připojený displej a přijímací modul RX5808. Tento projekt má za úkol měřit čas ulétnutého kola FPV dronu pomocí hodnoty RSSI z přijímacího modulu, podle které můžu analyzovat vzdálenost dronu od přijímače a tím určit kdy prolétnul v +- nějakém bodě. Od tohoto budu určovat čas daných kol.  

<p align="center">
<img src="https://media.discordapp.net/attachments/1098263330684162202/1196725308682944645/PXL_20240105_155428122.MP.jpg?ex=65b8ac4b&is=65a6374b&hm=17db8fb4e1685fb4a6aa4eebda0c159589d750873643357e4eb6c7ad3d0d13d7&=&format=webp&width=832&height=626" alt="drawing" width="300" />  
<p>

**Projekt je však zatím v hodně rané části, takže tolik kódu nemám, ale prakticky se zatím jedná jenom o přijímání signálu na jednom kanále a měření hodnoty RSSI. Samozřejmě chci domyslet počítání času, co přesně se bude zobrazovat na tom malém displeji a pokud budu vše stíhat tak udělat i stránku, na kterou se budete moct dostat, když se například z mobilu připojíte na ESP32, které bude mít hotspot a pomocí této stránky ovládat celý timer.**  

**!! Skripta podle toho potom řádně doplním o daný kód atd. !!**

### Klipper (Voron 0.2)
Tato ukázka spočívá v ukázání, jak Raspberry Pi nacházející se v tiskárně u mě doma dokáže ovládat 3D tiskárnu a zároveň sprostředkovávat print server pro ní.  

Přes interface Mainsail se přípojím do své tiskárny doma a začnu ji ovládat, popřípadě spustím tisk.  

<p align="center">
<img src="https://media.discordapp.net/attachments/1098263330684162202/1196725309676990545/PXL_20240105_125414212.MP.jpg?ex=65b8ac4b&is=65a6374b&hm=d7cadcff8e694ddae7c6d80dc30363205bcc9e8a25b576d58400152d006bc151&=&format=webp&width=471&height=626" alt="drawing" width="200" />  
<p>

**Tato ukázka pouze slouží jako příklad využití Raspberry Pi, nic z toho jsem nenaprogramoval, jediné co tak jsem pomáhal se sestavením této tiskárny (stavbou naší jednotky, ne celkově projektem) a následného nastavování, například kamery a také jsem tam vytvořil různá GCODE makra.**

### Čidla na chalupě
!! Potřebuji se domluvit s otcem, nemám přístup, nejspíš to ale vyjde !!  

**V celku se jedná o propojení více ESP vývojových desek, které spolu komunikují a posílají svá data z čidel na Grafanu. Toto také slouží pouze jako ukázka, tato práce je mého otce.**

## Zdroje
Raspberry Pi:  
* https://www.raspberrypi.com/  
* https://en.wikipedia.org/wiki/Raspberry_Pi  
* https://cs.wikipedia.org/wiki/Raspberry_Pi  
* https://github.com/raspberrypi  

Arduino:  
* https://www.arduino.cc/  
* https://store.arduino.cc/  
* https://cs.wikipedia.org/wiki/Arduino  
* https://en.wikipedia.org/wiki/Arduino  
* https://core-electronics.com.au/guides/history-of-arduino/ (obrázek)

ESP:  
* https://en.wikipedia.org/wiki/ESP32  
* https://en.wikipedia.org/wiki/ESP8266  
* https://gist.github.com/sekcompsci/2bf39e715d5fe47579fa184fa819f421  

Ostatní:  
* http://www.orangepi.org/  
* https://www.banana-pi.org/  
* https://wiki.radxa.com/  
* https://radxa.com/
