ff# 👑🪟Windows-Simplegood 👌👍🙌
> [!TIP]
> **Windows-Szimplajó telepítés beépített HDD/SSD lemezen: USB eszköz nélkül egyszerűbb, sokkal gyorsabb a Windows telepítés és nem igényli a Windows ISO fájl gyakori szokás szerinti
> kiírását külső programmal, mint pl. Rufus, vagy Media Creation Tool, magyarul nem kell telepítő média...
> <br><sup>'Csak' meglévő Windows kell hozzá😬</sup>**

> [!NOTE]
> Óriási erő kell 1 Windowst elrontani...igazából csak a nagyon gyengének sikerülhet. Annak is itt van ez!🥳🥳🥳
 
## Telepítő Partíció <sup>(USB adathordozó helyett)</sup>
1. Adathordozó (pl. USB) használata helyett a gépünk lemezén (ez a tárhely jóval gyorsabb, mint az USB) készítünk és használunk Windows telepítőt.
Ehhez lecsippentünk 1 „keveset” a meglévő lemez tárhelyünkből a gépünkön:
- Egér jobboldali gombbal ( 🖱️<sub>↖️</sub> ) klikk a Windows Start **&plusb;** tálcaikonon, majd a felugró listán **Lemezkezelés** választása. 
- A Lemezkezelés ablakban jobbgombos egér klikk a kéksávos **Windows (C:)** kötetre, majd a helyi menüben klikk: *Kötet zsugorítása*.<br>
   ![{47A9DFF5-E60C-4ECA-94F6-59443057CF51}](https://github.com/user-attachments/assets/88f57747-cd34-4f29-8abd-53538ee28ab2)
- A felugró ablakban a *zsugorítandó* méretet beállítjuk *10000 (tízezer) MB*-ra (ez kb.9,7 GB) majd jóváhagyjuk az új partíció készítést.(1-2+perc)<br>
   ![{3DEDB19B-E53F-4C3D-9578-5B79537053F4}](https://github.com/user-attachments/assets/2400f183-6a6f-4190-9ea4-ab75882d7ad7)
- Most az új (fekete sávos) **Lefoglalatlan partíció**ra jobb gombos egér klikk, majd a felugró listán *Új, egyszerű kötet* parancsra klikkelj. Végig klikkeljük - tovább, tovább... mindent elfogadva - a particionálási folyamatot, aminek eredményeként kapunk egy betűjellel ellátott kötetet/meghajtót „Új kötet” néven (ha particionálás közben nem neveztük át). A betűjelet particionálás közben automatikusan felajánlja a Lemezkezelő, általában **D:** a jó, ha nincs több partíció/meghajtó, ha van már ilyen, akkor a soron következő betű, pl. E:, F: stb. lesz a jó. Megfelelően követve a leírást a "fekete sávos" üres hely "kék sávos" partícióra változik... Bezárjuk a lemezkezelőt. Ha jól csináltuk, a Fájlkezelőben is megjelenik az új kötet (partíció/meghajtó), új betűjellel.

> [!NOTE]
> Íme a képen egy tipikus partíciós tábla, ahol a "tartalékként" is használt Windows telepítő ISO tartalma az **F:** (wininstall-nak elnevezett) partícióra/meghajtóra van helyezve (...és D: partíció is van külön a személyes fájloknak):
> <br>Lemezkezelő:
><br>
><img width="700" height="100" alt="{F115E94F-AC73-4425-8B7E-31F0B44B8772}" src="https://github.com/user-attachments/assets/530d2215-8923-4435-90a5-e107e1ed859e" />
><br>
>Fájlkezelő:
><br>
><img width="700" height="100" alt="{433B15AD-6701-4749-B84E-929F7C2D5A9B}" src="https://github.com/user-attachments/assets/2a631adf-44fb-4baa-bcd7-c07ad0c8bf31" />


## 📀 Windows ISO fájl
**Letöltjük** a netről a telepítő **lemezképet**, azaz a <tt>Windows ISO</tt> fájlt: 
- a Microsoft https://www.microsoft.com/hu-hu/software-download/windows11 oldaláról,
- vagy (egyszerűbben) a https://msdl.gravesoft.dev/#3262 címről
<br>😒 ...ezek szigorú hardverkövetelményű Windows 11 25H2 iso-k.

> [!WARNING]
> <sup>☝️ A **MS eredeti Windows 11** ISO-k (kivéve az Enterprise👌) csak a MS szerinti hardverkövetelményeknek, úgymint: secureboot, TPM2, minimum 4 GB RAM, 2009. után
> gyártott intel proci, vagy Win11 által támogatott Ryzen, stb. megfelelő gépre telepíthetők eredetiben, járj utána a neten, ha nem tudod, mi az. 
> Az egyik kritikus hardver a TPM2 biztonsági eszköz, ezt könnyen ellenőrizheted; jobb klikk a Start &plusb; ikonon, futtatás: **tpm.msc** begépelésére és <kbd>Enter</kbd>-re
> felugró ablakban részletes tájékoztatás jelenik meg a saját géped TPM eszközéről (ha 2-nél alacsonyabb spec.verziós, NEM lehet a gépedre eredeti MS Windows 11-et telepíteni  ((┬┬﹏┬┬)). 
> Pl. a Windows X-Lite vagy a ❤️ Win11Long_Alexa ISO-kban ki van kapcsolva a TPM2 ellenőr, tehát akadálytalanul települhet szinte
> bármely, viszonylag régebbi számítógépre is.</sup><br>
> ![{FFFC60A6-CE5D-4D29-A61A-8DD1B380D479}](https://github.com/user-attachments/assets/45b3486f-9301-40b7-9e64-758661921f1f)

> [!TIP]
> ...Letölthetünk megbízható Windows ISO-t más kedvenc helyünkről (jóval lazább hardverkövetelményekkel), pl.: https://windowsxlite.com/  (a Windows XLite kis hátránya, hogy csak angolul "beszél", de a telepítés után magyarítani lehet) vagy  itt a [Windows11Long_Alexa](https://github.com/mondomata/Windows11Long_Alexa) ❤️ (utóbbi magyar, nyomkövetőktől és hirdető/reklám progiktól mentes Windows 11!) Lényeges, hogy gyanús címről származó iso-t ne tölts le sehonnan; olvass utána...
  
## 📀 ISO kezelés
2. Az ISO tul.képpen speciálisan csomagolt állomány, amely könyvtárakat (mappákat), fájlokat tartalmaz (hasonlóan 1 tömörített állományhoz).
Megnyitás: a letöltött Windows.ISO-ra a Fájkezelőben jobb kattintás, majd **⨀Csatlakoztatás** választása (avagy pl. Win.10-en egyszerűen kattints 2x a fájlnévre <sup>(ha olyan régi Windowsod van, ami nem kezeli az iso-t, töltsd le a netről pl.a 7zip-et / https://7zip.org /, az jól kezeli...)</sup>:
   ![{C653C4A7-D76C-4838-835F-EB3B21020301}](https://github.com/user-attachments/assets/2778f1c2-580c-487f-8a53-571da122c13a)
 
3. Windows ISO tartalom, felépítés (tipikusan):
  ![{98ECB815-6026-4CE9-BA78-8EE0756B5A50}](https://github.com/user-attachments/assets/dc4f5c8c-2210-48ed-8dc1-5d1a762a79b7)

- az eredeti MS Windows.iso állományok kivétel nélkül tartalmazzák a fotón látható mappákat és fájlokat (méretek változók + egyéb is lehet),
- a telepítés indító fájl, a **setup.exe** zömmel a legfelső könyvtárban van, egyes telepítőknél - pl. Windows X-Lite - viszont nincs support mappa, illetve a *setup.exe a sources mappában* van.

4. A Telepítő Program felületen (*ez 1 Windows Telepítés című ablakban, a Windows telepítési folyamat során megjelenő grafikus, interaktív felület, amely végig vezet a telepítési folyamat meghatározott lépésein*) kritikus teendő az *új Windows partíciójának kijelölése*.
   <br>
   2 alapvető lehetőség van:
   - a meglévő helyére, a „régi” Windows törlésével, tiszta új Windows telepítünk (lásd 5. pont),
   - az eredeti Windows megtartása mellett egy második Windowst telepítünk (lásd 6. pont).
   - Mindkét esetben **segíthet** a telepítésben, ha a **C:** (Windows) partíció teljes méretét (GB) feljegyzed előtte (1 GB = 1024 MB!).

 ## ⚡'Tiszta' Új Windows<sup>haladóknak</sup>
5. **Felülírható a meglévő Windows így ('tiszta' telepítéssel!)**:
- **készíts a Windows Lemezkezelő**vel (1. pont szerint) egy új, kb. 10GB-os partíciót a lemezeden, adj neki **F:** betűjelet.  Csatold a fájlkezelőn a nevére kattintva (2.pont) a telepítő ISO-t (D: , vagy G: vagy hasonló meghajtón fog megnyílni), az ISO-ból **másold az összes mappát és fájlt** (fontos, hogy NEM az ISO-t, hanem a 2.pont szerint *megnyitott ISO tartalmát*!) az új, **F:** betűjelű üres partícióra.
- **Windows Helyreállítási Újraindítás**: ez a Tálca Start &plusb; ikonra, majd a <kbd>(|)</kbd>*Főkapcsoló* > **Újraindítás**-ra a <kbd>Shift</kbd> billentyű *nyomva tartása közben* rákattintva lehetséges. Másik mód: a Windows *Powershell (vagy Terminál)* programban ***shutdown /r /o*** begépelésével és <kbd>[&#8629;Enter]</kbd>-rel, (kb.1perc...)
- a **helyreállító menüben** (világoskék csempék) válaszd sorrendben a *Hibaelhárítás -> Speciális lehetőségek -> Parancssor* lehetőséget. (Win 10-nél a Parancssor elérése más is lehet e menüben.)
- Gépeld be a **Parancssor**ba, ahol látod majd az <tt> X:\Windows\System32> </tt>szöveget, hogy **F:\setup** és <kbd>[&#8629;Enter]</kbd>-rel **indul** a Windows telepítő. 😬 *Ha nem indul*, nem történik az <kbd>[&#8629;Enter]</kbd>-re semmi<sup>(mert hajlamos a Windows 'megkeverni' ilyenkor a meghajtókat)</sup>, egyszerűen *ismételd meg a parancs kiadását* így: **D:\setup** <kbd>[&#8629;Enter]</kbd> vagy **E:\setup** <kbd>[&#8629;Enter]</kbd>, stb. (**G H I**... betűvel) amíg rátalálva a helyes betűjelre azonnal elindul a telepítő.😁 
- Íme a "neheze" 😬🤞A Windows telepítő programban a meglévő/foglalt, **0.lemez - "?" (Windows) primary/elsődleges partíciót válaszd eszerint:** *...ha feljegyezted a C: meghajtó méretét (GB), akkor látni fogod: az a Windows partíció, amelyiknek a mérete egyezik a C:-vel; egyébként pedig általában a 0.lemez 'első' olyan primary partíciója a Windows-é, amelyik nagyobb 52 GB-nál, azaz több, mint 53000 MB... Ha régebben nem készült több partíció a gépeden, akkor egyértelmű lesz, mert a System/Rendszer partíció, valamint a Recovery/Helyreállítás partíción kívül mindössze 2 elsődleges/primary partíciód lesz a Telepítő szerint a lemezeden: a Windowsé, és a kb. 9.7 GB-os telepítő partíciód, amit az 1. pont szerint készítettél.* <sup>(Az alábbi képen egy lehetséges példát látsz a Telepítőből a Windows partíció választásra. Ezen a képen nincs 9.7 GB-os 'telepítős' partíció, de egyébként tipikus, a legnagyobb, a 0. lemez 3. partíció a Windows partíció...Nemigen lehet más esetben sem elrontani, mert túl kicsire nem enged tovább lépni...)</sup>
<img width="425" height="120" alt="{CB32250E-355D-4BDC-B982-A4E45EDCC5CF}" src="https://github.com/user-attachments/assets/26eafdf5-7834-430e-b06f-6750b2e27761" />

- A **<kbd>Tovább</kbd> majd a <kbd>[Telepítés]</kbd>** gombra kattintva megkezdődik a folyamat (visszavonhatatlan), a régi Windowst az új Windows felülírja (**🧨MINDENT TÖRÖL: személyes fájlok, programok, beállítások, stb!🧼**)
> [!TIP]
> 💡Windows tiszta telepítés lehetséges úgy is, hogy a megkezdése előtt egy másik - pl. százezer MB-os, azaz kb.100 GB-os Adat (D:) - partícióra másolod fontos fájlaid /doksik, képek, videók, bármi/.
> <sup>Ezt a partíciót is az 1.pontban írt leírás szerint készítsd el. (Tehát ehhez legalább 3 partíció kell, ilyesmit látsz az 1.pont képein.)</sup>
> A Telepítőben csak a "Windows" (C:) partíciót törlöd/írod felül, az "Adat" (D:) partíciót nem változtatod meg, az tartalmával együtt kezelhető marad az új Windows-zal (azonnal használható lesz a tartalma telepítés után)! Nagyon praktikus megoldás ez a nagyobb
> kapacitású - pl. 512 GB - lemezhez... Lényegesen kevésbé kockázatos a tiszta telepítés, mivel nem az egész lemezt, hanem csak a Windows partíciót írja felül a telepítő. 

## ⚡Két (2) Windows (dual boot)
6. **Két Windows 1 gépen: Régi és Új** (bárkinek ajánlott, nincs kockázata).
Végeredményként a telepítés után a gép indításakor a régi és az új Windows között választhatsz majd egy kettős -„dual boot”- menüből. *Nagyon egyszerű, de erősen ajánlott csak akkor alkalmazni, ha legalább 100 GB-os, vagy nagyobb szabad tárolóhely áll rendelkezésre a meglévő Windows-ban (C: meghajtó szabad hely méret).*
- A 2. pont szerint csatolt (Win.10 esetén a winrar vagy 7zip-pel megnyitott) ISO-ban a *setup.exe*-re kattintás után felugró ablakban azonnal indul a Windows telepítés.
- Válaszd a Windows telepítőben a meglévő  **Windows** partíciót (ez a 0.lemezen általában legnagyobb foglalt hely), majd abból vegyél le **Extend partition** gombbal egy min. 60000 (hatvanezer) MB-os új, "szabad/üres" partíciót. *Erre a szabad/üres partícióra kattintva kezdd meg a telepítést*...
   <sup>Ennek a megoldásnak később 2 folytatása is lehet: attól függően, h a használat alapján melyik tetszik jobban, a megtartani kívánt Windows Lemezkezelőjében törölheted a másik (inaktív) Windowsnak a partícióját, így automatikusan újra 1 Windows-os géped lesz.</sup>
> [!TIP]
> *Ha nem szeretnél a telepítés közben bajlódni az új, második Windows partícióval, a fentebb 1. pont szerint eljárva készíts még a telepítés megkezdése előtt egy min.60000 (hatvanezer)MB-os, NTFS partíciót, ezt válaszd majd a telepítő programban a partíciók közül!*

  Ennyi.🙌🙌🙌

> [!TIP]
> **USB tárolós ('pendrájvos') telepítés részletes leírását keresed? <a href="https://github.com/mondomata/Windows11Long_Alexa?tab=readme-ov-file#%EF%B8%8Ftelep%C3%ADt%C3%A9si-adathordoz%C3%B3-k%C3%A9sz%C3%ADt%C3%A9se-windows-on">Itt van ilyen is!</a> 🥳 Windows aktiválás is van a telepítőben.**
   
> [!IMPORTANT]
> ☝️☝️☝️<b>Fontos: NE piszkáld sem a Lemezkezelőben, sem a Windows Telepítőben a System (Rendszer) és Recovery (Helyreállítási) partíciót (hagyd úgy, ahogy vannak)!!!</b> Célszerű a
> fontosabb iratokat, fotókat, stb minden esetben kimenteni egy kártyára, vagy USB tárolóra (pendrájvra), bármilyen Windows telepítéskor! Meglévő Windows felülírásakor elvesznek a
> Windowsra telepített programok is, de természetesen az új Windowson ezek újra telepíthetők.
 
+1 Egy másik <A href="https://docs.google.com/document/d/12GJzHKCkH1YCkE6JRz90i2aesiUantKvXcLsYUD-QTw/edit?usp=drivesdk">step by step Windows 11 telepítés képekben...</a>

> [!CAUTION]
> Minden felelősség kizárva a szerző részéről (a leírtak kipróbáltak, jól működnek, viszont a gépek és emberek közötti különbségek akár kirívók is lehetnek).😁😁😁
