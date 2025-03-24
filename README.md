# Windows-Simplegood 👌👍🙌
Windows-Szimplajó telepítés (Nem csak egyszerűbb így, de sokkal gyorsabb is a telepítés menete általában, és nem igényli a Windows ISO média fájl gyakori szokás szerinti kiírását külső programmal, mint pl. Rufus, vagy Media Creation Tool...)

1. Adathordozó (pl. USB) használata helyett lecsippentünk 1 „keveset” a meglévő Windows tárhelyünkből a gépünkön:
- Egér jobboldali gombbal ( 🖱️← ) klikk a Windows 🪟Start tálcaikonon, majd Lemezkezelés választása. 
- A Lemezkezelőben jobb klikk a Windows (C:) meghajtóra, majd a helyi menüben "Kötet zsugorítása" lehetőség választása.
- A felugró ablakban a zsugorítandó méretet beállítjuk 10000 MB-ra (lásd még a helyes méretezéshez a 4. pontot is, ahol több ajánlott!), majd jóváhagyjuk az új partíció készítést. Az új Lefoglalatlan partícióra jobb klikk, majd „Új, egyszerű kötet” parancs választása és végik klikkeljük -tovább- a formázásái folyamatot, aminek eredményeként kapunk egy új betűjellel (D: vagy E:, stb) ellátott kb. 8-9 GB-os (4. pont esetén több) Kötetet/meghajtót („Új kötet” névvel). Bezárjuk a lemezkezelőt (ha jól csináltuk, a Fájlkezelőben megjelenik egy új, D: vagy E: meghajtó).
- Letöltjük a netről a Windows telepítő képfájlt/médiát (Windows ISO fájlt, a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról , vagy – speciális, magyar nyelvű telepítő médiát – a https://massgrave.dev , https://msdl.gravesoft.dev/#3113 címről, vagy más kedvenc helyünkről: https://windowsxlite.com/ ).
2. A letöltött Windows.ISO képfjálra
- a Fájkezelőben jobb kattintás, majd ⨀Csatlakoztatás választása,
- a megnyíló (csatolt) ablakban kijelöljük egérrel az összes mappát és fájlt (tehát az ISO teljes tartalmát), majd átmásoljuk (pl. Ctrl C, Ctrl V-vel) az egészet az 1. pontban létrehozott új kötetbe (D:, vagy E:, stb). Bezárunk minden programot, kivéve a Fájlkezelőt.
3. Windows telepítéséhez az "Új kötet" meghajtón lévő <b>setup.exe</b> fájlra kattintunk, máris megkezdődik az új Windows telepítés…
    Amikor a telepítőben az új Windows partícióját kell kijelölni 2 lehetőség van attól függően, hogy a meglévő helyére („régi” Windows törlésével, lásd 4.) akarjuk-e telepíteni, VAGY az eredeti megtartása mellett egy második Windowst akarunk (lásd 5.).
4. <b>Meglévő Windows „felülírás”</b>: válaszd ki azt a partíciót, amelyiken a meglévő Windows (általában C:) van, majd lépj tovább a telepítőben (ha nem látsz betűjeleket, a partíció méretéből lehet megítélni, melyik a megfelelő - általában a legnagyobb méretű - partíció, figyelmeztetni is fog a telepítő, hogy mindent törölsz)…
5. <b>Új, 2. Windows</b>: végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből. Válaszd a telepítőban az új, 1. pont szerint létrehozott, legalább 70000 MB-os partíciót (<i>ebben az esetben az 1.pont végrehajtásakor a zsugorítási méretet 10000 helyett ajánlott 70000 MB-ra /ha nincs elég hely a lemezen, akkor a minimum 15000 MB/ állítani!</i>), majd folytasd a telepítő-ablakban a telepítést hasonlóan a 4. ponthoz.
  Ennyi.🙌🙌🙌
  ___________________________________________________
6. Előfordul, hogy az új meghajtóra (2. pont) másolt <i>setup.exe nem indul el a Fájlkezelőből</i> a meglévő Windowson. Ez esetben kattints a Start menüre, majd a Kikapcs.ikonra <b>(|)</b> és a <b>SHIFT</b> gombot lenyomva tartva kattints az <b>Újraindítás</b>-ra. A gép újraindulás, egy spéci csempés menü jelenik meg, ahol válaszd a „Parancssor” (Command Prompt) lehetőségeket. Eredményként egy Parancsor ablak („fekete”) jelenik meg (általában X:\Windows szöveggel). Itt írd be: <b>C:\setup</b> és nyomj Entert. Megnyílik a Windows telepítő ablak, majd folytasd a 4., vagy 5. pontban írttal akaratod szerint. Egyetlen parancssori hiba lehetőség, hogy a setup.exe (telepítés futtató fájl) a spec. újraindítás miatt nem a C:-n, van, ezért ha a C:\setup +Enterre nem indul a telepítés, próbáld újra a D:\setup vagy E:\setup (csak 1 betű változtatás) paranccsal elindítani, amíg a Windows telepítés ablak megjelenik.
👌👌👌Fontos: NE piszkáld sem a Lemezkezelőben, sem a Windows Telepítőben a System és Recovery partíciót (hagyd úgy, ahogy vannak)!!! Célszerű a fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
 
+1 🥳 Windows aktiválás: https://drive.google.com/drive/folders/1m4t_hm1OKsj2OSDKkXJDh3a7ayw1g2iE

