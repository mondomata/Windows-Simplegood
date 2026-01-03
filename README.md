# Windows-Simplegood 👌👍🙌
Windows-Szimplajó telepítés (Nem csak egyszerűbb így, de sokkal gyorsabb is a telepítés menete általában, és nem igényli a Windows ISO média fájl gyakori szokás szerinti kiírását külső programmal, mint pl. Rufus, vagy Media Creation Tool...<sup>Windows kell hozzá😬</sup>)

## Partíció
1. Adathordozó (pl. USB) használata helyett lecsippentünk 1 „keveset” a meglévő Windows tárhelyünkből a gépünkön:
- Egér jobboldali gombbal ( 🖱️<sub>↖️</sub> ) klikk a Windows Start<kbd>![windowsbill](https://github.com/user-attachments/assets/6e47728d-5bf1-45a7-8cf9-5f72a2cb16a9)
</kbd> tálcaikonon, majd a felugró listán **Lemezkezelés** választása. 
- A Lemezkezelés ablakban jobb klikk a **Windows (C:)** kötetre, majd a helyi menüben <tt>Kötet zsugorítása</tt> lehetőség választása. ![{47A9DFF5-E60C-4ECA-94F6-59443057CF51}](https://github.com/user-attachments/assets/88f57747-cd34-4f29-8abd-53538ee28ab2)
- A felugró ablakban a zsugorítandó méretet beállítjuk 10000 MB-ra ![{3DEDB19B-E53F-4C3D-9578-5B79537053F4}](https://github.com/user-attachments/assets/2400f183-6a6f-4190-9ea4-ab75882d7ad7)
majd jóváhagyjuk az új partíció készítést. Most az új **Lefoglalatlan partíció**ra jobb klikk és <tt>Új, egyszerű kötet</tt> parancs választása (+ ajánlott NTFS helyett FAT partíciós rendszer beállítása). Végig klikkeljük -mindent elfogadva- a formázásái folyamatot, aminek eredményeként kapunk egy új betűjellel (D:, stb) ellátott közel 10 GB-os kötetet/meghajtót „Új kötet” néven (ha particionálás közben nem neveztük át).
Bezárjuk a lemezkezelőt. Ha jól csináltuk, a Fájlkezelőben is megjelenik az új kötet, új betűjellel.
## ISO fájl
- Letöltjük a netről a <tt>Windows ISO</tt> fájlt: a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról , vagy (egyszerűbben) a https://msdl.gravesoft.dev/#3262 címről, vagy más kedvenc helyünkről:
  https://windowsxlite.com/ https://github.com/mondomata/Windows11Long_Alexa❤️
  
  ☝️Figyelmeztetés: <sup>a MS eredeti Windows 11 ISO-k (kivéve az Enterprise👌) csak a MS szerinti hardverkövetelményeknek megfelelő gépre telepíthetők ezzel a módszerrel, járj utána a neten, ha nem tudod, mi az. Az egyik kritikus hardver a TPM2 biztonsági "csip"; jobb klikk a Startmenün, Futtatás: <tt>tpm.msc</tt> begépelése és Enter ![{FFFC60A6-CE5D-4D29-A61A-8DD1B380D479}](https://github.com/user-attachments/assets/45b3486f-9301-40b7-9e64-758661921f1f) felugró ablakban részletes tájékoztatás jelenik meg a géped TPM eszközéről.</sup> A Windows X-Lite ISO-ban, vagy a Win11Long_Alexa ISO-kban ki van kapcsolva ez a védelem, tehát akadálytalanul települhet szinte bármely, viszonylag régebbi számítógépre</sup>


##Telepítési módok

2. A letöltött Windows.ISO-ra
- a Fájkezelőben jobb kattintás, majd ⨀Csatlakoztatás választása, ![{C653C4A7-D76C-4838-835F-EB3B21020301}](https://github.com/user-attachments/assets/2778f1c2-580c-487f-8a53-571da122c13a) (Win 10 esetén leet, hogy az .iso csak külső programmal, pl. 7zip-pel nyitható meg.)

- a megnyíló (csatolt) ablakban kijelöljük egérrel az összes mappát és fájlt (tehát az ISO teljes tartalmát), majd átmásoljuk (pl. <kbd>Ctrl</kbd><kbd>C</kbd>, <kbd>Ctrl</kbd><kbd>V</kbd>-vel) az egészet az 1. pontban létrehozott új kötetbe. Bezárunk minden programot, kivéve a Fájlkezelőt.
  
3. Windows telepítés megkezdéséhez (*de csak az eredeti Windows megtartása mellett 5.pont szerint!*) az "Új kötet" meghajtóra másolt **setup.exe** fájlra kattintunk, felugró ablakban elindul a Windows telepítés progi…
  <span style="float:right">![{98ECB815-6026-4CE9-BA78-8EE0756B5A50}](https://github.com/user-attachments/assets/dc4f5c8c-2210-48ed-8dc1-5d1a762a79b7)</span> <sup>* az eredeti Windows.iso fájlok kivétel nélkül tartalmazzák a fotón látható mappákat és fájlokat, egyes telepítőknél - pl. módosított Windows X-Lite - viszont nincs support mappa, illetve a setup.exe a <code>sources</code> mappában van, abból indítható a telepítés</sup>

    A telepítőben a szerződés elfogadása (accept) után az új Windows partícióját kell kijelölni: 2 lehetőség van attól függően, hogy a meglévő helyére („régi” Windows törlésével, lásd 4.) akarjuk-e telepíteni, VAGY az eredeti megtartása mellett egy második Windowst akarunk (lásd 5.).
  
4. **Felülírható a meglévő Windows** így ("tiszta" telepítés!): készíts a Windows Partíciókezelővel egy új, kb. 10GB-os  FAT partíciót a lemezeden, adj neki **F:** betűjelet.  Csatold a fájlkezelőn a nevére kattintva a telepítő ISO-t (D: , vagy G: vagy hasonló meghajtón fog megnyílni), abból másold az összes mappát és fájlt az új, **F:** betűjelű partícióra. Windows Helyreállítási Módban (ezt <kbd>Shift</kbd>-et nyomva tartva a Start menüben a *Kikapcsolás*/*Újraindítás*-ra kattintva is el lehet érni), majd az újraindulás után megjelenő spec. menüben válaszd a *Hibaelhárítás -> Speciális lehetőségek -> Parancssor* lehetőséget. Gépeld be: **F:\setup** és [Enter]-rel indíthatod a Windows telepítőt. A telepítőben a meglévő **C:** Windows partíciót választva a régi Windowst az új Windows felülírja (<i>mindent töröl!!!</i>). Ha hibát jelez a Parancssor (nem indul a telepítő), egyszerűen ismételd meg a parancs kiadását így: <tt>D:\setup</tt> <kbd>[Enter]</kbd> vagy <tt>G:\setup</tt> <kbd>[Enter]</kbd>, stb. (abc betűivel) amíg rátalálva a helyes betűjelre elindul a telepítő. Windows 10-en meglehet, hogy az iso-t a fájlkezelő nem tudja megnyitni, ilyenkor töltsd le és használd pl. a **7zip** programot: https://www.7-zip.org/

5. <b>Új, 2. Windows (bárkinek ajánlott, nincs kockázata)</b>: végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből.
   A setup.exe-re kattintás után válaszd a Windows telepítőben a **Windows** partíciót, majd abból csípj le egy min. 60000 MB-os újabb, "üres" partíciót (<i>ebben az esetben erre az üres partícióra kattintva kezdd meg a telepítést), majd folytasd a telepítő-ablakban a telepítést 3.-4.ponthoz hasonlóan. <sup>Ennek a megoldásnak később 2 folytatása is lehet: attól függően, h a használat alapján melyik tetszik jobban, a megtartani kívánt Windows Lemezkezelőjében törölheted a másik (inaktív) Windowsnak a partícióját, így automatikusan újra 1 Windows-os géped lesz.</sup>
  
  Ennyi.🙌🙌🙌
<hr>
6. Előfordul, hogy az új meghajtóra (2. pont) másolt <i>setup.exe nem indul el a Fájlkezelőből</i> a meglévő Windowson, vagy indítás után hibát jelez.
Ez esetben kattints a Start menüre, majd a Kikapcs.ikonra <b><kbd>(|)</kbd></b> és a <b><kbd>SHIFT</kbd> gombot nyomva tartva</b> kattints az <b>Újraindítás</b>-ra. A gép újrainduláskor egy spéci csempés menü jelenik meg, ahol válaszd egymás után a <tt><b>Hibaelhárítás -> Speciális lehetőségek -> Parancssor</b></tt> csempeikont. Eredményként egy Parancssor ablak („fekete”) jelenik meg (általában X:\Windows szöveggel). Itt írd be: <b><code>D:\setup</code></b> és nyomj <kbd>Enter</kbd>t <sup>(egyes, nem gyári Microsoft Windows-oknál, mint a fent említett X-Lite, a kiadandó parancs: <code>D:\sources\setup</code>)</sup>. Megnyílik a Windows telepítő ablak, majd folytasd a 4., vagy 5. pontban írttal akaratod szerint. Egyetlen parancssori hiba lehetőség, hogy a setup.exe (telepítés futtató fájl) a spec. újraindítás miatt nem a D:-n, van, ezért ha a D:\setup +<kbd>Enter</kbd>re nem indul a telepítés, próbáld újra 1 betű változtatással: <code>E:\setup</code> vagy <code>F:\setup</code>(abc rend szerinti betűjelekkel ...) elindítani, amíg a Windows telepítés ablak megjelenik.
   
☝️☝️☝️<b>Fontos: NE piszkáld sem a Lemezkezelőben, sem a Windows Telepítőben a System (Rendszer) és Recovery (Helyreállítási) partíciót (hagyd úgy, ahogy vannak)!!!</b> Célszerű a fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
 
+1 🥳 Windows aktiválás a fenti Win11Long_Alexa telepítőben, 
egy Windows 11 telepítés képekben...:

https://docs.google.com/document/d/12GJzHKCkH1YCkE6JRz90i2aesiUantKvXcLsYUD-QTw/edit?usp=drivesdk

