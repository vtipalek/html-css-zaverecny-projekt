# Závěrečný projekt

*Zadání pro závěrečný projekt v kurzu HTML a CSS (blended) od Czechitas*

Tvým úkolem je nakódovat kompletní  **responzivní** stránku **restaurace Bříško**.
- v HTML máš připravený obsah, ale musíš si ho obalit dalšími prvky podle potřeby a přidat CSS třídy
- v CSS jsou připravené proměnné pro barvy, ale zbytek už si musíš nastavit sama

Ukázky výsledku jsou v kořenové složce projektu, kde je i video *ukazka-responzivniho-chovani.mp4*, na kterém je vidět stránka ve všech responzivních variantách.

Není-li v zadání níže uvedený nějaký rozměr (padding, margin) nebo jiné nastavení specificky uvedeno, **odhadni** ho tak, aby to vypadalo podobně jako na obrázku s ukázkou výsledku.

**Pokud něčemu nebudeš rozumět, zeptej se na Discordu nebo na konzultační lekci lektora nebo koučů.**


## Doporučení

- Obsah je rozdělený na hlavičku, hero sekci (banner), jídelní lístek, rozvážku jídla a patičku.
- V CSS nastyluj nejprve věci, které jsou společné pro všechny varianty webu - nastavení písma, velikosti nadpisů, tlačítko a *container* pro obsah (viz dále), nastavení pro sekce obecně.
- Doporučujeme stylovat po jednotlivých sekcích - můžeš klidně napřeskáčku, ale vyber si jednu sekci, uprav si pro ni HTML a pak v CSS začni mobilní variantou a nakonec přidej media query pro tablet a desktop.
- Když se budeš soustředit vždy na jednu sekci, nebudeš zahlcená tím, co se děje ve zbytku webu.
- Až vyřešíš všechny responzivní změny pro jednu sekci, můžeš se přesunout na další.


## Responzivní breakpointy

Stránka má tři responzivní varianty, říkejme jim zjednodušeně *mobil*, *tablet* a *desktop*.

- **tablet** od `768px` a víc
- **desktop** od `1100px` a víc


## Prvky společné pro celou stránku

### Písmo

- [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) - písmo pro nadpisy `h1` a `h2`
- [DM Sans](https://fonts.google.com/specimen/DM+Sans) - písmo pro všechny ostatní texty na stránce
- připoj písma z Google Fonts do stránky a v CSS nastav na příslušné prvky

#### Základní text pro celou stránku (nastavený na body)

- písmo **DM Sans**
- velikost písma: `1.125rem` nastavené
- výška řádku `1.4` nastavené
- barva `--color-text` nastavené

#### Nadpis h1

- písmo **Playfair Display**
- velikost písma: -
  - mobil: `3.5rem` nastavené
  - tablet: `4rem` nastavené
  - desktop: `5rem` nastavené
- tloušťka písma `400` nastavené
- výška řádku `1` nastavené

#### Nadpisy h2

- písmo **Playfair Display**
- velikost písma: -
  - mobil: `2.5rem` nastavené
  - tablet: `3rem` nastavené
  - desktop: `3.5rem` nastavené
- tloušťka písma `500` nastavené
- výška řádku `1.2` nastavené

#### Nadpisy h3

- písmo **DM Sans**
- velikost písma `1.5rem` nastavené
- tloušťka písma `600` nastavené
- výška řádku `1.2` nastavené


### Sekce -

Následující platí obecně pro **sekce** a **patičku** stránky. nastavené

- padding nahoře a dole `50px` nastavené
- od tabletu dál se padding zvětší na `80px` nastavené

### Container -

Obsah jednotlivých sekcí (včetně hlavičky a patičky) je zůžený do pruhu s nastavenou maximální šířkou, který je vycentrovaný uprostřed stránky. nastavené

Container přidej vždy do každé sekce takto: nastavené
```html
<section>
  <div class="container">

  </div>
</section>
```

- **Na mobilu:** -
  - maximální šířka `540px` nastavené
  - vycentrován horizontálně uprostřed stránky nastavené
  - padding vpravo a vlevo `20px` nastavené
- **Od tabletu** a výše: -
  - nastavená maximální šířka se změní na `1100px` nastavené

### Tlačítko -

Tlačítko se chová také responzivně, mění se mu velikost písma a padding. nastavené

- **Na mobilu:** -
  - `display: inline-block;`, aby šel tlačítku nastavit padding nastavené
  - padding nahoře a dole `15px`, vpravo a vlevo `30px` nastavené
  - velikost písma `1rem` nastavené
  - tloušťka písma `600` nastavené
  - písmo je nepodtržené nastavené
  - barva textu bílá nastavené
  - barva pozadí `--color-primary` nastavené
  - při najetí myší (nebo klávesnicí) se barva pozadí změní na `--color-primary-dark` nastavené
  - border radius `100vw` (tlačítko bude na koncích vždy perfektně kulaté, nezávisle na tom, jak bude velké) nastavené
- **Od tabletu** výše: -
  - padding se změní na `20px` nahoře a dole, `40px` vpravo a vlevo nastavené
  - velikost písma se změní na `1.125rem` nastavené

![Tlačítko](assets/tlacitko.png)


## Hlavička stránky - ALE VYRIEŠIŤ MARGIN

- celá hlavička má padding nahoře a dole `20px` nastavené ALE VYRIEŠIŤ MARGIN

**Logo**: -
- na mobilu má výšku `35px` nastavené
- na desktopu má výšku `45px` nastavené

**Položky menu (odkazy)**: -
- **Na mobilu:** -
  - `display: inline-block;` aby jim šel nastavit padding nastavené
  - padding nahoře a dole `10px`, vlevo a vpravo `15px` nastavené
  - velikost písma `1.25rem` nastavené
  - tloušťka písma `500` nastavené
  - písmo není podtržené nastavené
  - barva textu `--color-secondary-dark` nastavené
  - border radius `100vw` (aby bylo tlačítko na koncích kompletně kulaté) nastavené
  - při najetí myší (nebo klávesnicí) se barva pozadí nastaví na `--color-secondary-bright` nastavené
- **Na tabletu:** -
  - padding se změní na `10px` nahoře a dole, `20px` vlevo a vpravo nastavené
- **Na desktopu:** -
  - padding se změní na `15px` nahoře a dole, `30px` vlevo a vpravo nastavené

![Menu](assets/menu.png)

Na mobilu jsou logo a menu **pod sebou**, od tabletu výše jsou **vedle sebe**, logo úplně vlevo, menu úplně vpravo. nastavené


## Hero banner

- obrázek na pozadí kompletně pokrývá plochu banneru nastavené
- sekce s bannerem má padding nahoře a dole:
  - **na mobilu** `100px`
  - **na tabletu** `120px`
  - **na desktopu** `150px`
- mezi nadpisem a textem, a mezi textem a tlačítkem je rozestup `30px` nastavené
- text mezi nadpisem a tlačítkem: -
  - **na mobilu** velikost textu `1.125rem` nastavené
  - **od tabletu** výše je velikost textu `1.25rem` nastavené

![Hero banner](assets/hero.png)


## Sekce: Jídelní lístek -

- mezi nadpisem a kartičkami je rozestup `40px` nastavené
- kartičky jsou: -
  - **na mobilu** pod sebou nastavené
  - **na tabletu** 2 vedle sebe a pod nimi další 2 (nápověda viz dále) nastavené
  - **na desktopu** všechny 4 kartičky vedle sebe nastavené
- mezi kartičkami je rozestup `30px` nastavené
- kartička má padding nahoře a dole `30px`, vpravo a vlevo `20px` nastavené
- vycentrovaný text nastavené
- rámeček `1px` barvou `--color-secondary-bright` nastavené
- zakulacení rohů velikosti `--radius` nastavené
- **ikona** uvnitř kartičky má velikost `40px` x `40px` nastavené
- **nadpis** v kartičce je barvou `--color-secondary` nastavené
- **odkaz** na spodku kartičky je barvou `--color-primary`, je nepodtržený, ale podtrhne se při najetí myší (nebo klávesnicí) nastavené
- vertikální rozestup mezi prvky v kartičce je `20px` nastavené

![Jídelní lístek](assets/jidelni-listek.png)

### Nápověda pro rozložení kartiček na tabletu:

- kartičky dej do flexboxu nastavené
- na flexboxu zapni zalamování pomocí `flex-wrap: wrap;` nastavené
- to znamená, že když se prvky do flexboxu nevejdou, na konci řádku se zalomí a budou pokračovat na dalším řádku - tak uděláš 2 řady kartiček nastavené
- kartičkám musíš nastavit správnou šířku tak, aby se přesně vešly a zalomily se tam, kde potřebuješ nastavené
- musíš počítat i s mezerou mezi kartičkami, takže když chceš dvě kartičky vedle sebe, musí být šířka kartičky `(100% - 30px) / 2` - použij `calc()` nastavené
- nezapomeň na desktopové variantě zalamování ve flexboxu zase vypnout pomocí `flex-wrap: nowrap;` a nastavit kartičky na správnou šířku, aby se vešly čtyři vedle sebe

![Jídelní lístek na tabletu](assets/jidelni-listek-tablet.png)


## Sekce: Rozvoz jídla

Sekce je rozdělená na dvě poloviny, které jsou na mobilu pod sebou, na tabletu a desktopu vedle sebe a jsou stejně široké. Když jsou sloupce vedle sebe, je mezi nimi rozestup `60px`. NASTAVIT

Sekce má barvu pozadí `--color-section-bg`. nastavené

⚠️ **Pozor:** NASTAVIT
Pro obrázek s jídlem přidej element `<picture>` a zajisti, aby: -
- **na mobilu** se zobrazoval široký obrázek *rozvoz-na-sirku.jpg* nastavené
- **od tabletu** výše se zobrazoval vysoký obrázek *rozvoz-na-vysku.jpg* nastavené

![Picture](assets/picture.png)

- mezi prvky vedle obrázku jsou rozestupy `40px` NASTAVIT
- **ikony** jsou velké `40px` x `40px` nastavené
- **text vedle ikon** má: -
  - velikost `1.25rem` nastavené
  - tloušťku písma `500` nastavené
  - barvu `--color-secondary-dark` nastavené

![Rozvoz jídla](assets/rozvoz.png)


## Patička - ? ALE ASI INÁ TRIEDA NA LOGO A MENU

- pozadí patičky `--color-footer-bg` nastavené
- barva textu `--color-secondary-light` nastavené
- barva odkazů v patičce `--color-secondary-bright` nastavené
- výška loga `40px` nastavené
- patička je rozdělená na dvě poloviny: -
  - logo a adresa nastavené /časom možno iná trieda/
  - menu a copyright nastavené /časom možno iná trieda/
- **na mobilu** jsou obě poloviny pod sebou nastavené
- **od tabletu** a výše jsou obě poloviny vedle sebe na opačných koncích patičky nastavené
- když jsou prvky nad sebou, je mezi nimi rozestup `20px` nastavené

![Patička](assets/paticka.png)


## Ukázky výsledku

Takto vypadají celé stránky v jednotlivých responzivních rozloženích.

### Mobil

![Ukázka výsledku pro mobil](ukazka-vysledku-mobil.png)

### Tablet

![Ukázka výsledku pro tablet](ukazka-vysledku-tablet.png)

### Desktop

![Ukázka výsledku pro desktop](ukazka-vysledku-desktop.png)
