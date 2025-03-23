# Windows-Simplegood
Windows-Szimplajó (telepítés)

1. Adathordozó (pl. USB) használata helyett lecsippentünk 1 „keveset” a meglévő Windows tárhelyünkből a gépünkön:
- Jobb klikk a Startmenün, majd Lemezkezelés választása. (Nem csak egyszerűbb, de sokkal gyorsabb is a telepítés menete általában!)
- Jobb klikk a Lemezkezelőben a C: (Windows) meghajtóra, majd Zsugorítás lehetőség választása.
- A felugró ablakban a zsugorítás méretet beállítjuk 10000 MB-ra (lásd még a helyes méretezéshez a 4. pontot is, ahol kb. 70000 MB kell!), majd jóváhagyjuk az új partíció készítést. Az új partícióra jobb klikk, majd „Új, egyszerű kötet” parancs választása és végik klikkeljük a formázásái folyamatot, aminek eredményeként kapunk egy új betűjellel (D: vagy E:, stb) ellátott kb. 8-9 GB-os (4. pont esetén több) Kötetet/meghajtót („Új kötet” névvel). Bezárjuk a lemezkezelőt.
- Letöltjük a netről a Windows telepítő képfájlt/médiát (Windows ISO fájlt, a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról , vagy – speciális, magyar nyelvű telepítő médiát – a https://massgrave.dev -ről, vagy más kedvenc helyünkről).
2. A letöltött Windows.ISO képfjálra
- a Fájkezelőben jobb kattintás, majd „Csatolás” választása,
- a megnyíló (csatolt) ablakban kijelöljük az összes mappát és fájlt (tehát az ISO teljes tartalmát), majd átmásoljuk (pl. Ctrl C, Ctrl V-vel) az egészet az 1. pontban létrehozott új kötetbe (D:, E:, stb). Bezárunk minden programot, kivéve a Fájlkezelőt.
3. Windows telepítéséhez az új meghajtón lévő <b>setup.exe</b> fájlra kattintunk, máris megkezdődik az új Windows telepítés… Amikor a telepítőben az új Windows partícióját kell kijelölni 2 lehetőség van attól függően, hogy második Windowst akarunk (5.), vagy a meglévő helyére („régi” Windows törlésével) akarjuk-e (4.) telepíteni.
4. <b>Meglévő Windows „felülírás”</b>: válaszd ki azt a partíciót, amelyiken a meglévő Windows (általában C:) van, majd lépj tovább a telepítőben (ha nem látsz betűjeleket, a partíció méretéből lehet megítélni, melyik a megfelelő partíció, figyelmeztetni is fog a telepítő, hogy mindent törölsz)…
5. <b>Új, 2. Windows</b>: (végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből) válaszd ki az új, 1. pont szerint létrehozott, legalább 60 GB-os partíciót (ebben az esetben az 1.pont végrehajtásakor a zsugorítási méretet 10000 helyett ajánlott kb. 70000 MB-ra állítani!), majd folytasd a telepítő-ablakban a telepítést. Ennyi.
  ___________________________________________________
6. Előfordul, hogy az új meghajtóra (2. pont) másolt setup.exe nem indul el a Fájlkezelőből a meglévő Windowson. Ez esetben kattints a Start-ra, majd a Kikapcs. Ikonra, és a SHIFT gomb lenyomásával együtt kattints az „Újraindítás”-ra. Így a gép újra induláskor egy spéci menü jelenik meg, ahol válaszd a „Karbantartás”, majd „Parancssor” lehetőségeket. Eredményként egy Parancsor ablak („fekete”) jelenik meg (általában X:\Windows szöveggel). Itt írd be: C:\setup és nyomj Entert*. Megnyílik a Windows telepítő ablak, majd folytasd a 3. (új Windows) vagy 4. (meglévő Windows felülírása) pontban írttal akaratod szerint. (*Egyetlen hiba lehetőség, ami miatt nem indul el a telepítés, hogy a setup.exe (telepítés futtató fájl) a spec. újraindítás miatt nem a C:-n, van, ezért próbáld újra a D:\setup vagy E:\setup (csak 1 betű változtatás) paranccsal elindítani a telepítést, amíg a telepítő ablak meg nem jelenik…)
👌👌👌Fontos: célszerű a fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
