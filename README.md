# 🪟Windows-Simplegood 👌👍🙌
**Windows-Szimplajó telepítés beépített HDD vagy SSD-ről: nem csak egyszerűbb így, de sokkal gyorsabb is a telepítés menete és nem igényli a Windows ISO média fájl gyakori szokás szerinti kiírását külső programmal, mint pl. Rufus, vagy Media Creation Tool...<sup>'Csak' meglévő Windows kell hozzá😬</sup>)**

## Telepítő Partíció <sup>USB tárhely helyett</sup>
1. Adathordozó (pl. USB) használata helyett lecsippentünk 1 „keveset” a meglévő Windows tárhelyünkből a gépünkön:
- Egér jobboldali gombbal ( 🖱️<sub>↖️</sub> ) klikk a Windows Start<kbd>![windowsbill](https://github.com/user-attachments/assets/6e47728d-5bf1-45a7-8cf9-5f72a2cb16a9)
</kbd> tálcaikonon, majd a felugró listán **Lemezkezelés** választása. 
- A Lemezkezelés ablakban jobb klikk a **Windows (C:)** kötetre, majd a helyi menüben <tt>Kötet zsugorítása</tt> lehetőség választása.
   ![{47A9DFF5-E60C-4ECA-94F6-59443057CF51}](https://github.com/user-attachments/assets/88f57747-cd34-4f29-8abd-53538ee28ab2)
- A felugró ablakban a zsugorítandó méretet beállítjuk 10000 MB-ra
   ![{3DEDB19B-E53F-4C3D-9578-5B79537053F4}](https://github.com/user-attachments/assets/2400f183-6a6f-4190-9ea4-ab75882d7ad7)
majd jóváhagyjuk az új partíció készítést.
- Most az új **Lefoglalatlan partíció**ra jobb klikk és <tt>Új, egyszerű kötet</tt> parancs választása (+ ajánlott NTFS helyett FAT partíciós rendszer beállítása). Végig klikkeljük -mindent elfogadva- a formázásái folyamatot, aminek eredményeként kapunk egy új betűjellel (D:, stb) ellátott közel 10 GB-os kötetet/meghajtót „Új kötet” néven (ha particionálás közben nem neveztük át).
Bezárjuk a lemezkezelőt. Ha jól csináltuk, a Fájlkezelőben is megjelenik az új kötet, új betűjellel.

## Windows ISO fájl
Letöltjük a netről a <tt>Windows ISO</tt> fájlt: a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról , vagy (egyszerűbben) a https://msdl.gravesoft.dev/#3262 címről (ezek szigorú hardverkövetelményű Windows 11 25H2 iso-k), vagy más kedvenc helyünkről (jóval lazább hardverkövetelményekkel): https://windowsxlite.com/ vagy https://github.com/mondomata/Windows11Long_Alexa❤️
  
  ☝️Figyelmeztetés: <sup>a MS eredeti Windows 11 ISO-k (kivéve az Enterprise👌) csak a MS szerinti hardverkövetelményeknek (secureboot, TPM2, minimum 4 GB RAM, "2019.év+os gyártású" intel proci, vagy Win11 által támogatott Ryzen, stb.) megfelelő gépre telepíthetők ezzel a módszerrel, járj utána a neten, ha nem tudod, mi az. 
  Az egyik kritikus hardver a TPM2 biztonsági "csip"; jobb klikk a Startmenün, futtatás: <tt>tpm.msc</tt> begépelése és Enter 
  ![{FFFC60A6-CE5D-4D29-A61A-8DD1B380D479}](https://github.com/user-attachments/assets/45b3486f-9301-40b7-9e64-758661921f1f) felugró ablakban részletes tájékoztatás jelenik meg a géped TPM eszközéről.</sup> 
  A Windows X-Lite ISO-ban, vagy a Win11Long_Alexa ISO-kban ki van kapcsolva ez a védelem, tehát akadálytalanul települhet szinte bármely, viszonylag régebbi számítógépre</sup>

## ISO kezelési módok
2. A letöltött Windows.ISO-ra...
- a Fájkezelőben jobb kattintás, majd ⨀Csatlakoztatás választása, ![{C653C4A7-D76C-4838-835F-EB3B21020301}](https://github.com/user-attachments/assets/2778f1c2-580c-487f-8a53-571da122c13a)
- Win 10 esetén lehet, hogy az .iso csak külső programmal, pl. 7zip-pel nyitható meg. (https://7zip.org)
 
3. ISO tartalom, felépítés:
  ![{98ECB815-6026-4CE9-BA78-8EE0756B5A50}](https://github.com/user-attachments/assets/dc4f5c8c-2210-48ed-8dc1-5d1a762a79b7)
- az eredeti Windows.iso fájlok kivétel nélkül tartalmazzák a fotón látható mappákat és fájlokat (méretek változók + egyéb is lehet),
- egyes telepítőknél - pl. Windows X-Lite - viszont nincs support mappa, illetve a **setup.exe a sources mappában** van, amivel indítható a telepítés...

4. A telepítőben majd a szerződés elfogadása (accept) után az *új Windows partícióját kell kijelölni*:
   2 lehetőség van attól függően, hogy
   - a meglévő helyére, a „régi” Windows törlésével akarjuk-e telepíteni (lásd 5.),
   - VAGY az eredeti megtartása mellett egy második Windowst akarunk (lásd 6.).

 ## "Tiszta" Új Windows <sup>haladóknak</sup>
5. **Felülírható a meglévő Windows így ("tiszta" telepítés!)**: készíts a Windows Partíciókezelővel (1.pont) egy új, kb. 10GB-os  FAT partíciót a lemezeden, adj neki **F:** betűjelet.  Csatold a fájlkezelőn a nevére kattintva (2.pont) a telepítő ISO-t (D: , vagy G: vagy hasonló meghajtón fog megnyílni), abból másold az összes mappát és fájlt az új, **F:** betűjelű üres partícióra.
**Windows Helyreállítási Módban** újraindulás után (ezt a Tálca/Start menüben a <kbd>Shift</kbd>-et nyomva tartva a <kbd>(|)</kbd>*Kikapcsolás*/*Újraindítás*-ra kattintva lehet elindítani, vagy *Powershell* programban a **shutdown /r /o** begépelésével és <kbd>[Enter]</kbd>-rel), a megjelenő spec. menüben (világoskék csempék) válaszd sorrendben a *Hibaelhárítás -> Speciális lehetőségek -> Parancssor* lehetőséget. Gépeld be: **F:\setup** és <kbd>[Enter]</kbd>-rel indíthatod a Windows telepítőt.
A Windows telepítés ablakban a meglévő **C:** Windows partíciót válaszd (ha inaktív marad a telepítő gomb, töröld ezt a partíciót a Törlés/Delete gombbal, és így az új üres partícióra telepíthetsz), a Telepítés gombbal a régi Windowst az új Windows felülírja (**mindent töröl!!!**). Ha hibát jelez a Parancssor (nem indul a telepítő), egyszerűen ismételd meg a parancs kiadását így: <tt>D:\setup</tt> <kbd>[Enter]</kbd> vagy <tt>G:\setup</tt> <kbd>[Enter]</kbd>, stb. (abc betűivel) amíg rátalálva a helyes betűjelre elindul a telepítő. Windows 10-en meglehet, hogy az iso-t a fájlkezelő nem tudja megnyitni, ilyenkor töltsd le és használd pl. a **7zip** programot: https://www.7-zip.org/

## 2 Windows (dual boot)
6. **Két Windows 1 gépen: Régi és Új** (bárkinek ajánlott, nincs kockázata). Végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből. *Nagyon egyszerű, de erősen ajánlott csak akkor alkalmazni, ha legalább 100 GB-os, vagy nagyobb szabad tárolóhely áll rendelkezésre a meglévő Windows-ban (C: meghajtó szabad hely méret).*
   A 2. pont szerint csatolt ISO-ból a *setup.exe*-re kattintás után felugró ablakban azonnal indul a Windows telepítés. Válaszd a Windows telepítőben a **Windows** partíciót, majd abból vegyél le **Extend partition** gombbal egy min. 60000 MB-os újabb, "üres" partíciót. *Erre az üres partícióra kattintva kezdd meg a telepítést*...
   <sup>Ennek a megoldásnak később 2 folytatása is lehet: attól függően, h a használat alapján melyik tetszik jobban, a megtartani kívánt Windows Lemezkezelőjében törölheted a másik (inaktív) Windowsnak a partícióját, így automatikusan újra 1 Windows-os géped lesz.</sup>
*Ha nem szeretnél a telepítés közben bajlódni az új, második Windows partícióval, a fentebb 1. pont szerint eljárva készíts még a telepítés megkezdése előtt egy min.60000 MB-os, NTFS partíciót!*
  Ennyi.🙌🙌🙌
<hr>
   
☝️☝️☝️<b>Fontos: NE piszkáld sem a Lemezkezelőben, sem a Windows Telepítőben a System (Rendszer) és Recovery (Helyreállítási) partíciót (hagyd úgy, ahogy vannak)!!!</b> Célszerű a fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
 
+1 🥳 Windows aktiválás a fenti Win11Long_Alexa telepítőben, 
egy Windows 11 telepítés képekben...:

https://docs.google.com/document/d/12GJzHKCkH1YCkE6JRz90i2aesiUantKvXcLsYUD-QTw/edit?usp=drivesdk

