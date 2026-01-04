# 🪟Windows-Simplegood 👌👍🙌
**Windows-Szimplajó telepítés beépített HDD/SSD lemezről: USB nélkül egyszerűbb, sokkal gyorsabb a Windows telepítés és nem igényli a Windows ISO média fájl gyakori szokás szerinti kiírását külső programmal, mint pl. Rufus, vagy Media Creation Tool...<sup>'Csak' meglévő Windows kell hozzá😬</sup>)**

## Telepítő Partíció <sup>USB adathordozó helyett</sup>
1. Adathordozó (pl. USB) használata helyett a gépünk lemezén (ez a tároló általában jóval gyorsabb, mint az USB) készítünk és használunk Windows telepítőt.
Ehhez lecsippentünk 1 „keveset” a meglévő lemez tárhelyünkből a gépünkön:
- Egér jobboldali gombbal ( 🖱️<sub>↖️</sub> ) klikk a Windows Start<kbd>![windowsbill](https://github.com/user-attachments/assets/6e47728d-5bf1-45a7-8cf9-5f72a2cb16a9)
</kbd> tálcaikonon, majd a felugró listán **Lemezkezelés** választása. 
- A Lemezkezelés ablakban jobbgombos egér klikk a kék **Windows (C:)** kötetre, majd a helyi menüben klikk: *Kötet zsugorítása*.<br>
   ![{47A9DFF5-E60C-4ECA-94F6-59443057CF51}](https://github.com/user-attachments/assets/88f57747-cd34-4f29-8abd-53538ee28ab2)
- A felugró ablakban a zsugorítandó méretet beállítjuk 10000 (tízezer) MB-ra (ez kb.9,7 GB) majd jóváhagyjuk az új partíció készítést.<br>
   ![{3DEDB19B-E53F-4C3D-9578-5B79537053F4}](https://github.com/user-attachments/assets/2400f183-6a6f-4190-9ea4-ab75882d7ad7)
- Most az új (fekete) **Lefoglalatlan partíció**ra jobb gombos egér klikk, majd a felugró listán *Új, egyszerű kötet* parancsra klikkelj (+ ajánlott NTFS helyett FAT32 fájlrendszerű partíciós tábla beállítása). Végig klikkeljük - tovább, tovább... mindent elfogadva - a particionálási folyamatot, aminek eredményeként kapunk egy új betűjellel ellátott kötetet/meghajtót „Új kötet” néven (ha particionálás közben nem neveztük át). A betűjelet particionálás közben ajánla a Lemezkezelő, általában **D:** a jó, ha nincs több partíció és/vagy CD/DVD lejátszó a gépben<sup>ami általában D:-re van csatolva)</sup>, ha van már ilyen, akkor a soron következő betű, pl. E:, F: stb. lesz a jó. Megfelelően követve az itt írtakat a "fekete" üres hely "kék" (logikai) partícióra változik... Bezárjuk a lemezkezelőt. Ha jól csináltuk, a Fájlkezelőben is megjelenik az új kötet (meghajtó), új betűjellel.

Íme a képen egy tipikus partíciós tábla, ahol a "tartalékként" is használt Windows telepítő ISO az **F:** (wininstall-nak elnevezett) partícióra/meghajtóra van helyezve:
<br>Lemezkezelő:
<br>
<img width="700" height="100" alt="{F115E94F-AC73-4425-8B7E-31F0B44B8772}" src="https://github.com/user-attachments/assets/530d2215-8923-4435-90a5-e107e1ed859e" />
<br>
Fájlkezelő:
<br>
<img width="700" height="100" alt="{433B15AD-6701-4749-B84E-929F7C2D5A9B}" src="https://github.com/user-attachments/assets/2a631adf-44fb-4baa-bcd7-c07ad0c8bf31" />


## Windows ISO fájl
Letöltjük a netről a "telepítőképet", azaz a <tt>Windows ISO</tt> fájlt: 
- a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról,
- vagy (egyszerűbben) a https://msdl.gravesoft.dev/#3262 címről
(ezek szigorú hardverkövetelményű Windows 11 25H2 iso-k).
> [!TIP]
> ...Letöltünk Windows ISO-t más kedvenc helyünkről (jóval lazább hardverkövetelményekkel), pl.: https://windowsxlite.com/ (kis hátránya, hogy angolul "beszél", de a telepítés után
> magyarítani lehet) vagy https://github.com/mondomata/Windows11Long_Alexa❤️ (utóbbi magyar, nyomkövetőktől és hirdető/reklám progiktól mentes Windows 11!)
  
> [!WARNING]
> ☝️Figyelmeztetés: a MS eredeti Windows 11 ISO-k (kivéve az Enterprise👌) csak a MS szerinti hardverkövetelményeknek, úgymint: secureboot, TPM2, minimum 4 GB RAM, 2019. után
> gyártott intel proci, vagy Win11 által támogatott Ryzen, stb.) megfelelő gépre telepíthetők ezzel a módszerrel, járj utána a neten, ha nem tudod, mi az. 
> Az egyik kritikus hardver a TPM2 biztonsági eszköz; jobb klikk a Startmenün, futtatás: **tpm.msc** begépelésére és <kbd>Enter</kbd>-re
> felugró ablakban részletes tájékoztatás jelenik meg a saját géped TPM eszközéről (ha 2-nél alacsonyabb verziós, NEM lehet a gépedre eredeti MS Windows 11-et telepíteni). 
> A Windows X-Lite ISO-ban, vagy a ❤️ Win11Long_Alexa ISO-kban ki van kapcsolva ez a védelem, tehát akadálytalanul települhet szinte bármely, viszonylag régebbi számítógépre is.
> ![{FFFC60A6-CE5D-4D29-A61A-8DD1B380D479}](https://github.com/user-attachments/assets/45b3486f-9301-40b7-9e64-758661921f1f)

## ISO csatlakoztatási módok
2. Az ISO-k tul.képpen spec. csomagolt állományok, amelyek könyvtárakat (mappákat), fájlokat tartalmaznak, megnyitásuk speciális.
A letöltött Windows.ISO-ra...
- a Fájkezelőben jobb kattintás, majd ⨀Csatlakoztatás választása:
   ![{C653C4A7-D76C-4838-835F-EB3B21020301}](https://github.com/user-attachments/assets/2778f1c2-580c-487f-8a53-571da122c13a)
- Win 10 esetén lehet, hogy az ISO csak külső programmal, pl. winrar, 7zip nyitható meg. (https://7zip.org)
 
3. Windows ISO tartalom, felépítés (tipikusan):
  ![{98ECB815-6026-4CE9-BA78-8EE0756B5A50}](https://github.com/user-attachments/assets/dc4f5c8c-2210-48ed-8dc1-5d1a762a79b7)

- az eredeti MS Windows.iso állományok kivétel nélkül tartalmazzák a fotón látható mappákat és fájlokat (méretek változók + egyéb is lehet),
- egyes telepítőknél - pl. Windows X-Lite - viszont nincs support mappa, illetve a telepítés indító **setup.exe a sources mappában** van.

4. A telepítőben a legfontosabb, kritikus teendő: az *új Windows partícióját kell kijelölni*.
   2 alapvető lehetőség van attól függően, hogy
   - a meglévő helyére, a „régi” Windows törlésével (tiszta telepítéssel) akarjuk-e telepíteni (lásd 5.),
   - VAGY az eredeti Windows megtartása mellett egy második Windowst akarunk (lásd 6.).

 ## "Tiszta" Új Windows <sup>haladóknak</sup>
5. **Felülírható a meglévő Windows így ("tiszta" telepítés!)**:
- készíts a Windows Partíciókezelővel (1.pont) egy új, kb. 10GB-os  FAT32 fájlrendszerű partíciót a lemezeden, adj neki **F:** betűjelet.  Csatold a fájlkezelőn a nevére kattintva (2.pont) a telepítő ISO-t (D: , vagy G: vagy hasonló meghajtón fog megnyílni), az ISO-ból másold az összes mappát és fájlt az új, **F:** betűjelű üres partícióra.
- **Windows Helyreállítási Módban újraindulás** után (ezt a módot a Tálca/Start menüben a <kbd>Shift</kbd>-et nyomva tartva a <kbd>(|)</kbd>*Kikapcsolás*/*Újraindítás*-ra kattintva lehet elindítani, vagy *Powershell* programban a **shutdown /r /o** begépelésével és <kbd>[Enter]</kbd>-rel),
- a megjelenő spec. menüben (világoskék csempék) válaszd sorrendben a *Hibaelhárítás -> Speciális lehetőségek -> Parancssor* lehetőséget. (Win 10-nél a Parancssor /Command Prompt/ elérése eltérő lehet.) Gépeld be: **F:\setup** és <kbd>[Enter]</kbd>-rel indíthatod a Windows telepítőt.
- A Windows telepítés ablakban a meglévő **C:** Windows partíciót válaszd (ha inaktív marad a telepítő gomb, töröld ezt a partíciót a Törlés/Delete gombbal, és így az új üres partícióra telepíthetsz), a Telepítés gombbal a régi Windowst az új Windows felülírja (**mindent töröl!!!**).
- ^_^  Ha hibát jelez a Parancssor (nem indul a telepítő), egyszerűen ismételd meg a parancs kiadását így: <tt>D:\setup</tt> <kbd>[Enter]</kbd> vagy <tt>G:\setup</tt> <kbd>[Enter]</kbd>, stb. (abc betűivel) amíg rátalálva a helyes betűjelre elindul a telepítő. Windows 10-en meglehet, hogy az iso-t a fájlkezelő nem tudja megnyitni, ilyenkor töltsd le és használd pl. a **7zip** programot: https://www.7-zip.org/

## 2 Windows (dual boot)
6. **Két Windows 1 gépen: Régi és Új** (bárkinek ajánlott, nincs kockázata).
Végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből. *Nagyon egyszerű, de erősen ajánlott csak akkor alkalmazni, ha legalább 100 GB-os, vagy nagyobb szabad tárolóhely áll rendelkezésre a meglévő Windows-ban (C: meghajtó szabad hely méret).*
- A 2. pont szerint csatolt ISO-ból a *setup.exe*-re kattintás után felugró ablakban azonnal indul a Windows telepítés.
- Válaszd a Windows telepítőben a **Windows** partíciót, majd abból vegyél le **Extend partition** gombbal egy min. 60000 MB-os újabb, "üres" partíciót. *Erre az üres partícióra kattintva kezdd meg a telepítést*...
   <sup>Ennek a megoldásnak később 2 folytatása is lehet: attól függően, h a használat alapján melyik tetszik jobban, a megtartani kívánt Windows Lemezkezelőjében törölheted a másik (inaktív) Windowsnak a partícióját, így automatikusan újra 1 Windows-os géped lesz.</sup>
> [!TIP]
> *Ha nem szeretnél a telepítés közben bajlódni az új, második Windows partícióval, a fentebb 1. pont szerint eljárva készíts még a telepítés megkezdése előtt egy min.60000 MB-os, NTFS >partíciót!*

  Ennyi.🙌🙌🙌

> [!TIP]
> USB tárolós ('pendrájvos') telepítés részletes leírását keresed? Itt van ilyen is: https://github.com/mondomata/Windows11Long_Alexa
   
> [!IMPORTANT]
> ☝️☝️☝️<b>Fontos: NE piszkáld sem a Lemezkezelőben, sem a Windows Telepítőben a System (Rendszer) és Recovery (Helyreállítási) partíciót (hagyd úgy, ahogy vannak)!!!</b> Célszerű a
> fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a
> Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
 
+1 🥳 Windows aktiválás is van a fenti Win11Long_Alexa telepítőben.
Egy step by step Windows 11 telepítés képekben... https://docs.google.com/document/d/12GJzHKCkH1YCkE6JRz90i2aesiUantKvXcLsYUD-QTw/edit?usp=drivesdk

> [!CAUTION]
> Minden felelősség kizárva a szerző részéről (a leírtak kipróbáltak, jól működnek, viszont a gépek és emberek közötti különbségek akár kirívók is lehetnek).😁😁😁
