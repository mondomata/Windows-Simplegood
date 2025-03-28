# Windows-Simplegood 👌👍🙌
Windows-Szimplajó telepítés (Nem csak egyszerűbb így, de sokkal gyorsabb is a telepítés menete általában, és nem igényli a Windows ISO média fájl gyakori szokás szerinti kiírását külső programmal, mint pl. Rufus, vagy Media Creation Tool...<sup>Windows kell hozzá😬</sup>)

1. Adathordozó (pl. USB) használata helyett lecsippentünk 1 „keveset” a meglévő Windows tárhelyünkből a gépünkön:
- Egér jobboldali gombbal ( 🖱️<sub>↖️</sub> ) klikk a Windows 🪟Start tálcaikonon, majd Lemezkezelés választása. 
- A Lemezkezelés ablakban jobb klikk a <code>Windows (C:)</code> kötetre, majd a helyi menüben <tt>Kötet zsugorítása</tt> lehetőség választása. ![{47A9DFF5-E60C-4ECA-94F6-59443057CF51}](https://github.com/user-attachments/assets/88f57747-cd34-4f29-8abd-53538ee28ab2)
- A felugró ablakban a zsugorítandó méretet beállítjuk 10000 MB-ra ![{3DEDB19B-E53F-4C3D-9578-5B79537053F4}](https://github.com/user-attachments/assets/2400f183-6a6f-4190-9ea4-ab75882d7ad7)
<sup>(lásd még a helyes méretezéshez az 5. pontot, ahol több ajánlott!)</sup>, majd jóváhagyjuk az új partíció készítést. Most az új "Lefoglalatlan partícióra" jobb klikk és „Új, egyszerű kötet” parancs választása. Végig klikkeljük -mindent elfogadva- a formázásái folyamatot, aminek eredményeként kapunk egy új betűjellel (D:, stb) ellátott kb. 8-9 GB-os (4. pont esetén több) Kötetet/meghajtót „Új kötet” néven. Bezárjuk a lemezkezelőt. Ha jól csináltuk, a Fájlkezelőben is megjelenik az új kötet, új betűjellel.
- Letöltjük a netről a Windows telepítő fájlt (ez a <tt>Windows ISO</tt> fájl: a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról , vagy (egyszerűbben) a https://msdl.gravesoft.dev/#3113 címről, vagy más kedvenc helyünkről: https://windowsxlite.com/ ❤️
  
  (☝️Figyelmeztetés: a MS eredeti Windows 11 ISO-k (kivéve az IoT Enterprise👌 https://drive.massgrave.dev/en-us_windows_11_iot_enterprise_version_24h2_x64_dvd_3a99b72b.iso) csak TPM2 biztonsági eszközzel ellátott gépre telepíthetők ezzel a módszerrel, járj utána a neten, ha nem tudod, mi az. Saját gépeden ellenőrizheted a meglétét így: jobb klikk a Startmenün, Futttatás, majd <tt>tpm.msc</tt> begépelése és Enter ![{FFFC60A6-CE5D-4D29-A61A-8DD1B380D479}](https://github.com/user-attachments/assets/45b3486f-9301-40b7-9e64-758661921f1f) <sup>felugró ablakban részletes tájékoztatás jelenik meg a géped TPM eszközéről. A Windows X-Lite ISO-ban ki van kapcsolva ez a védelem, tehát akadálytalanul települhet szinte bármely, nem túl régi számítógépre</sup>
2. A letöltött Windows.ISO-ra
- a Fájkezelőben jobb kattintás, majd ⨀Csatlakoztatás választása, ![{C653C4A7-D76C-4838-835F-EB3B21020301}](https://github.com/user-attachments/assets/2778f1c2-580c-487f-8a53-571da122c13a)

- a megnyíló (csatolt) ablakban kijelöljük egérrel az összes mappát és fájlt (tehát az ISO teljes tartalmát), majd átmásoljuk (pl. Ctrl C, Ctrl V-vel) az egészet az 1. pontban létrehozott új kötetbe (D:,stb). Bezárunk minden programot, kivéve a Fájlkezelőt.
3. Windows telepítés megkezdéséhez az "Új kötet" meghajtóra másolt <b><code>setup.exe</code></b> fájlra kattintunk, felugró ablakban elindul a Windows telepítés progi… ![{98ECB815-6026-4CE9-BA78-8EE0756B5A50}](https://github.com/user-attachments/assets/dc4f5c8c-2210-48ed-8dc1-5d1a762a79b7) <sup>* az eredeti Windows.iso fájlok kivétel nélkül tartalmazzák a fotón látható mappákat és fájlokat, egyes telepítőknél - pl. módosított Windows X-Lite - viszont nincs support mappa, illetve a setup.exe a <code>sources</code> mappában van, abból indítható a telepítés</sup>

    A telepítőben a szerződés elfogadása (accept) után az új Windows partícióját kell kijelölni: 2 lehetőség van attól függően, hogy a meglévő helyére („régi” Windows törlésével, lásd 4.) akarjuk-e telepíteni, VAGY az eredeti megtartása mellett egy második Windowst akarunk (lásd 5.).
4. <b>Meglévő Windows „felülírás”(csak gyakorlottaknak ajánlott!)</b>: A setup.exe-re kattintás után a Windows telepítő ablakban válaszd ki azt a partíciót, amelyiken a meglévő Windows (általában C:) van, majd lépj tovább a telepítőben (ha nem látsz betűjeleket, a partíció méretéből lehet megítélni, melyik a megfelelő - általában a legnagyobb méretű - partíció, figyelmeztetni fog a telepítő, hogy mindent törölsz, hagyd jóvá)…
5. <b>Új, 2. Windows(bárkinek ajánlott, nincs kockázata)</b>: végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből.A setup.exe-re kattintás után válaszd a Windows telepítőben az új, 1. pont szerint létrehozott, legalább 70000 MB-os "Új kötet" partíciót (<i>ebben az esetben az 1.pont végrehajtásakor a zsugorítási méretet 10000 helyett ajánlott 70000 MB-ra<sup> /ha nincs elég hely a lemezen, akkor a minimum 15000 MB/</sup> állítani!</i>), majd folytasd a telepítő-ablakban a telepítést 3.-4.ponthoz hasonlóan. <sup>Ennek a megoldásnak később 2 folytatása is lehet: attól függően, h a használat alapján melyik tetszik jobban, a megtartani kívánt Windows Lemezkezelőjében törölheted a másik (inaktív) Windowsnak a partícióját, így automatikusan újra 1 Windows-os géped lesz.</sup>
  
  Ennyi.🙌🙌🙌
  ___________________________________________________
6. Előfordul, hogy az új meghajtóra (2. pont) másolt <i>setup.exe nem indul el a Fájlkezelőből</i> a meglévő Windowson. Ez esetben kattints a Start menüre, majd a Kikapcs.ikonra <b>(|)</b> és a <b>SHIFT</b> gombot lenyomva tartva kattints az <b>Újraindítás</b>-ra. A gép újrainduláskor egy spéci csempés menü jelenik meg, ahol válaszd a „Parancssor” (Command Prompt) lehetőségeket. Eredményként egy Parancssor ablak („fekete”) jelenik meg (általában X:\Windows szöveggel). Itt írd be: <b><code>C:\setup</code></b> és nyomj <code>Enter</code>t <sup>(egyes, nem gyári Microsoft Windows-oknál, mint a fent említett X-Lite, a kiadandó parancs: <code>C:\sources\setup</code>)</sup>. Megnyílik a Windows telepítő ablak, majd folytasd a 4., vagy 5. pontban írttal akaratod szerint. Egyetlen parancssori hiba lehetőség, hogy a setup.exe (telepítés futtató fájl) a spec. újraindítás miatt nem a C:-n, van, ezért ha a C:\setup +Enterre nem indul a telepítés, próbáld újra 1 betű változtatással: <code>D:\setup</code> vagy <code>E:\setup</code> elindítani, amíg a Windows telepítés ablak megjelenik.
   
☝️☝️☝️<b>Fontos: NE piszkáld sem a Lemezkezelőben, sem a Windows Telepítőben a System és Recovery partíciót (hagyd úgy, ahogy vannak)!!!</b> Célszerű a fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
 
+1 🥳 Windows aktiválás (magyar nyelvű szkript): https://tinyurl.hu/PHaI

