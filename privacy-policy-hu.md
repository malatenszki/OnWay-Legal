# Adatvédelmi Tájékoztató

**Szolgáltatás:** OnWay — közlekedési POI figyelmeztető alkalmazás
**Adatkezelő:** Malatenski David, magánszemély (Szerbia)
**Kapcsolat:** onway.help@proton.me
**Hatályos:** 2026-04-13
**Verzió:** 1.0

---

## 1. Az Adatkezelő

A jelen Adatvédelmi Tájékoztató (a továbbiakban: **Tájékoztató**) hatálya az OnWay alkalmazás használata során kezelt személyes adatokra terjed ki.

| Adatkezelő | Malatenski David (magánszemély) |
|---|---|
| Ország | Szerbia |
| E-mail | onway.help@proton.me |

Az adatkezelésre az **Európai Parlament és a Tanács (EU) 2016/679 rendelete (GDPR)** közvetlenül alkalmazandó. A GDPR-ban nem szabályozott kérdésekben az **információs önrendelkezési jogról és az információszabadságról szóló 2011. évi CXII. törvény (Infotv.)** — különösen annak 52-60/A. §-ai a Nemzeti Adatvédelmi és Információszabadság Hatóság (NAIH) előtti eljárás tekintetében — irányadó.

## 2. A Tájékoztató célja

A jelen Tájékoztató célja, hogy átlátható módon bemutassa:
- milyen személyes adatokat kezelünk a Szolgáltatás nyújtása során
- milyen célból és milyen jogalapon kezeljük ezeket az adatokat
- meddig tároljuk az adatokat
- kikkel osztjuk meg az adatokat
- milyen jogok illetik meg a Felhasználót az adatai kapcsán
- hogyan léphet kapcsolatba velünk az adatai kezelése ügyében

## 3. A kezelt személyes adatok köre

Az OnWay működéséhez az alábbi személyes adatok kezelése szükséges:

### 3.1 Pszeudonim eszközazonosító (Felhasználói fiók)

- **Adatkör:** Pszeudonim UUID (univerzális egyedi azonosító), amelyet a Supabase anonim hitelesítési rendszere generál az Alkalmazás első indításakor
- **Jogalap:** A GDPR 6. cikk (1) bekezdés f) pont — **az Adatkezelő jogos érdeke** egy működő, díjmentes POI figyelmeztető szolgáltatás nyújtására, amely az egyedi eszközök megkülönböztetését igényli (pl. bejelentés-tulajdonlás, szavazási jogosultság, csalás elleni intézkedések)
- **Érdekmérlegelés:** A Felhasználó magánszférához való érdeke kiegyensúlyozódik az Adatkezelő azon érdekével, hogy működő és moderálható szolgáltatást nyújthasson. Az eszközazonosító nem kötődik közvetlenül a Felhasználó személyazonosságához, és az Adatkezelő nem ötvözi más adatforrásokkal profilalkotási célra — így a Felhasználó érdekei nem élveznek elsőbbséget. A Felhasználó a 8. szakaszban foglaltak szerint tiltakozási jogot gyakorolhat.
- **Cél:** A Felhasználó eszközének megkülönböztetése a Szolgáltatás működése során (pl. report-ok tulajdonosa, szavazási jogosultság)
- **Megjegyzés:** Az eszközazonosító NEM tartalmaz közvetlenül azonosító adatot (nincs név, e-mail, telefon, stb.) — ez **pszeudonim** adatkezelés, amely azonban a GDPR Recital 26 értelmében a rendelet hatálya alá tartozik

### 3.2 Eszközinformációk

- **Adatkör:** Platform (iOS / Android), alkalmazás-verzió, utolsó aktivitás időpontja
- **Jogalap:** A GDPR 6. cikk (1) bekezdés b) pont — szerződés teljesítése + f) pont — **jogos érdek** (a szolgáltatás minőségének ellenőrzése, hibakeresés)
- **Cél:** Hibakeresés, platform-kompatibilitás biztosítása, frissítési értesítések

### 3.3 Helyadatok (GPS)

- **Adatkör:** Szélességi és hosszúsági fok, irányérték (heading), sebesség
- **Jogalap (előtér):** A GDPR 6. cikk (1) bekezdés f) pont — **az Adatkezelő jogos érdeke** egy pozíció-alapú POI figyelmeztető szolgáltatás nyújtására. Az előtérben futó helymeghatározást az operációs rendszer helymeghatározási engedélye (iOS/Android permission) hatékony hozzájárulási mechanizmusként kezeljük; a Felhasználó ezt bármikor visszavonhatja a készülék beállításai között.
- **Jogalap (háttér):** A GDPR 6. cikk (1) bekezdés a) pont — **kifejezett, külön in-app hozzájárulás**, mivel a háttérben történő helymeghatározás adatvédelmi szempontból szenzitívebb
- **Cél:** A térkép megfelelő középre hozása, a közeli kamerákról és POI-król való valós idejű figyelmeztetés
- **Megőrzés:** A valós idejű GPS-adatokat az Alkalmazás **kizárólag a Felhasználó eszközén** dolgozza fel, a szerverre **nem kerülnek elmentésre**, kivéve, ha a Felhasználó kifejezetten bejelentést (report) küld, vagy ha figyelmeztetési esemény (alert_event) kerül naplózásra (lásd 3.4-3.5)

#### 3.3.1 A háttérben történő helymeghatározás hozzájárulás-kezelése

A háttérben történő helymeghatározáshoz szükséges hozzájárulás kezelése a GDPR 7. cikke és a GDPR 4. cikk 11. pontja szerinti követelmények betartásával történik:

- **Hozzájárulás megadása:** A háttérben történő helymeghatározás kizárólag egy **külön in-app megerősítő képernyő** elfogadása után aktiválódik, amely egyértelműen tájékoztat az adatkezelés céljáról. Az operációs rendszer saját „Always Allow" engedélye önmagában nem elegendő — az in-app hozzájárulás az Adatkezelő által dokumentálva marad.
- **Hozzájárulás visszavonása:** A Felhasználó a hozzájárulást **bármikor, ugyanolyan egyszerűséggel** visszavonhatja az Alkalmazás Beállítások menüjében található kapcsolóval, amely a jövőbeli háttérben történő adatgyűjtést haladéktalanul leállítja. A visszavonás a készülék oldali OS engedély visszavonásával is ekvivalens hatású.
- **A visszavonás joghatása:** A visszavonás nem érinti a korábbi, hozzájárulás alapján jogszerűen folytatott adatkezelés jogszerűségét. A már korábban rögzített figyelmeztetési események (alert_events) a 4. szakasz szerinti megőrzési időben kerülnek kezelésre.

### 3.4 Felhasználói bejelentések (Reports)

- **Adatkör:** Bejelentés típusa (rendőr / radar / ellenőrzés / baleset), helyzete (lat/lng), iránya, létrehozás időpontja, lejárat időpontja, a létrehozó pszeudonim eszközazonosítója
- **Jogalap:** A GDPR 6. cikk (1) bekezdés f) pont — **az Adatkezelő és más Felhasználók jogos érdeke** a valós idejű közlekedési információk megosztására és fogadására. Érdekmérlegelés: a bejelentéseket maga a Felhasználó hozza létre önkéntesen, azok nyilvános helyszínekre és közérdekű eseményekre vonatkoznak (nem tartalmaznak harmadik személyek személyes adatait), és pszeudonim eszközazonosítón keresztül kapcsolódnak a közzétevőhöz.
- **Cél:** Más Felhasználók figyelmeztetése az aktuális útviszonyokról

### 3.5 Figyelmeztetési események (Alert Events)

- **Adatkör:** Figyelmeztetés forrása (fix kamera vagy report), forrás ID-ja, kiváltás időpontja, helyszíne, iránya, sebessége, a figyelmeztetett eszköz pszeudonim azonosítója
- **Jogalap:** A GDPR 6. cikk (1) bekezdés f) pont — **jogos érdek** (a Szolgáltatás minőségének folyamatos javítása, statisztikai és térképes elemzés, forgalmi gócpontok meghatározása)
- **Cél:** A Szolgáltatás fejlesztése, forgalmi minták elemzése (heatmap), csaláselhárítás, visszaélések megelőzése
- **Jogos érdek mérlegelés:** Az adatok elemzése pszeudonim eszközazonosító szintjén történik, a Felhasználó személyazonossága ebből nem állapítható meg.

### 3.6 Szavazatok (Report Votes)

- **Adatkör:** Bejelentés azonosítója, szavazó pszeudonim eszközazonosítója, szavazat értéke (megerősítés / cáfolat)
- **Jogalap:** A GDPR 6. cikk (1) bekezdés f) pont — **jogos érdek** a közösségi moderáció, a hamis bejelentések kiszűrése és a Szolgáltatás integritásának biztosítása céljából
- **Cél:** A bejelentések közösségi moderálása

### 3.7 Opcionális becenév

- **Adatkör:** A Felhasználó által a Beállításokban megadott rövid, publikus megjelenítendő név
- **Jogalap:** A GDPR 6. cikk (1) bekezdés a) pont — **kifejezett hozzájárulás** (a mező opcionális, és a Felhasználó aktívan beír egy értéket)
- **Cél:** A Felhasználó bejelentéseinek és hozzájárulásainak publikus attribúciója
- **Megjegyzés:** A Felhasználó bármikor törölheti vagy módosíthatja a becenevet. Az Adatkezelő javasolja, hogy a Felhasználó ne adja meg valódi nevét.

### 3.8 Admin audit napló (csak admin felhasználókra)

- **Adatkör:** Adminisztrátor azonosítója, végrehajtott művelet, célobjektum, időbélyeg, IP cím
- **Jogalap:** A GDPR 6. cikk (1) bekezdés f) pont — **az Adatkezelő jogos érdeke** a rendszerbiztonság, a felelősségre vonhatóság és a csalásmegelőzés terén
- **Cél:** Adminisztrációs műveletek visszakövethetősége

### 3.9 Amit NEM kezelünk

Az OnWay **kifejezetten nem kezel** az alábbiakat:
- Valódi név, e-mail cím, telefonszám (a Felhasználó anonim marad, kivéve ha önkéntesen becenevet ad meg)
- Bankkártya vagy fizetési adatok
- Közösségi média profilok
- Különleges kategóriájú adatok (egészségügyi, származási, vallási, stb.)
- Gyermekek adatai (az Alkalmazás 16+ korhatárú, lásd 11. pont)

## 4. Adatmegőrzési idő

| Adattípus | Megőrzési idő |
|---|---|
| Pszeudonim eszközsor (`devices`) | A Felhasználó törlési kérelméig, vagy **24 hónap** inaktivitás után automatikus anonimizálás |
| Bejelentések (`reports`) | Aktív állapotban: a lejárat időpontjáig (45 perc — 8 óra). Lejárat után: **90 nap**, majd automatikus törlés |
| Szavazatok (`report_votes`) | A Felhasználó fiók törlésekor anonimizálódnak; a darabszámok megmaradnak, csak az attribúció szűnik meg |
| Kamera megerősítések (`camera_confirmations`) | A Felhasználó fiók törlésekor anonimizálódnak; a darabszámok megmaradnak, csak az attribúció szűnik meg |
| Figyelmeztetési események (`alert_events`) | **12 hónap**, majd automatikus **anonimizálás és aggregált statisztikai formába** átalakítás, amely a GDPR (26) preambulumbekezdése értelmében **már nem minősül személyes adatnak** |
| Admin audit napló (`admin_audit_log`) | **5 év** (felelősségi és biztonsági okokból) |
| GPS-adatok (valós idejű) | **NEM tárolódnak** a szerveren (kivéve a fenti eseteket) |

## 5. Adatfeldolgozók és adattovábbítás

Az Adatkezelő a Szolgáltatás nyújtása érdekében az alábbi adatfeldolgozókat veszi igénybe:

### 5.1 Fő adatfeldolgozó: Supabase

- **Név:** Supabase Inc.
- **Szerep:** Adatbázis, hitelesítés, felhőalapú backend szolgáltatás
- **Tárolás helye:** **Amazon Web Services (AWS) eu-west-3 régió — Párizs, Franciaország** (EU területén belüli tárolás)
- **Jogalap:** A GDPR 28. cikk szerinti adatfeldolgozói szerződés (DPA) keretében
- **További információ:** https://supabase.com/privacy

### 5.2 Térképes csempe-szolgáltatás: OpenStreetMap

- **Név:** OpenStreetMap Foundation (OSMF)
- **Szerep:** Térképi csempék (raster tiles) szolgáltatása
- **Tárolás helye:** Európai Unió területén működő szerverek
- **Adatkör:** A Felhasználó eszközének IP-címe és térkép-csempe kérése
- **További információ:** https://osmfoundation.org/wiki/Privacy_Policy

### 5.3 Platform szolgáltatók (mobil store)

- **Apple Inc.** (App Store — iOS platformra) — USA, EU-US Data Privacy Framework alapján
- **Google LLC** (Google Play Store — Android platformra) — USA, EU-US Data Privacy Framework alapján

### 5.4 Push értesítés (jövőbeli funkció)

Ha az Alkalmazás push értesítési funkciót vezet be, a push token és az értesítés tartalma az APNs vagy FCM szolgáltatáson keresztül kerül továbbításra. **Jelenleg ez a funkció még nem aktív.**

### 5.5 Adatok nem kerülnek értékesítésre

Az Adatkezelő a Felhasználó személyes adatait **nem adja el, nem adja bérbe és nem továbbítja marketing célra** harmadik félnek.

## 6. Nemzetközi adattovábbítás

Az Adatkezelő elsődlegesen **az Európai Unió területén belül** (AWS eu-west-3, Párizs) tárolja az adatokat. A fentiekben megjelölt EU-n kívüli adatfeldolgozók (pl. Apple, Google) esetén az adattovábbítás az alábbi megfelelőségi mechanizmusok alapján történik:

- **EU-US Data Privacy Framework** (az Európai Bizottság 2023/1795 végrehajtási határozata)
- **Standard Contractual Clauses (SCC)** — Európai Bizottság 2021/914 határozata
- Ha szükséges, kiegészítő technikai és szervezési intézkedések (titkosítás, pszeudonimizáció)

## 7. Biztonsági intézkedések

Az Adatkezelő az adatok biztonsága érdekében az alábbi intézkedéseket alkalmazza:

- **Titkosított adattovábbítás** (HTTPS/TLS 1.2+) minden kliens-szerver kommunikációban
- **Titkosított tárolás** (AES-256 at-rest titkosítás) a Supabase infrastruktúrában
- **Row Level Security (RLS)** az adatbázis szintjén
- **Pszeudonimizáció** (pszeudonim UUID, nem közvetlen azonosítók)
- **Admin audit log** minden adminisztrációs művelet rögzítésére
- **Kétfaktoros hitelesítés** (2FA) az adminisztrátori hozzáférésekhez
- **Automatikus biztonsági mentés** napi rendszerességgel

## 8. Az érintett (Felhasználó) jogai

A GDPR alapján a Felhasználót az alábbi jogok illetik meg:

### 8.1 Hozzáféréshez való jog (GDPR 15. cikk)

A Felhasználó jogosult tájékoztatást kérni arról, hogy kezeljük-e az adatait, és ha igen, milyen adatait.

### 8.2 Helyesbítéshez való jog (GDPR 16. cikk)

A Felhasználó jogosult a pontatlan adatok helyesbítését kérni.

### 8.3 Törléshez való jog (GDPR 17. cikk — „elfeledtetéshez való jog")

A Felhasználó bármikor kérheti a személyes adatainak törlését. Ez az Alkalmazásban a **„Adataim törlése"** funkcióval (Beállítások → Adatvédelem) is elvégezhető, vagy az Adatkezelőnek küldött e-maillel.

### 8.4 Adatkezelés korlátozásához való jog (GDPR 18. cikk)

A Felhasználó kérheti, hogy az adatai kezelését az Adatkezelő korlátozza az alábbi esetekben:
- Ha vitatja az adatok pontosságát
- Ha az adatkezelés jogellenes és a Felhasználó nem a törlést kéri
- Ha az Adatkezelőnek már nincs szüksége az adatokra, de a Felhasználónak szüksége van rájuk jogi igényeinek érvényesítéséhez

### 8.5 Adathordozhatósághoz való jog (GDPR 20. cikk)

A Felhasználó jogosult a rá vonatkozó adatok **gépileg olvasható formátumban** (JSON) történő megszerzésére.

### 8.6 Tiltakozáshoz való jog (GDPR 21. cikk)

A Felhasználó tiltakozhat az adatok jogos érdeken alapuló kezelése ellen (különösen a 3.5 szakasz szerinti Alert Events adatkezelés).

### 8.7 Hozzájárulás visszavonásához való jog (GDPR 7. cikk (3) bekezdés)

Ha az adatkezelés jogalapja a Felhasználó hozzájárulása (pl. háttérben történő helymeghatározás), a Felhasználó **bármikor díjmentesen visszavonhatja** a hozzájárulást.

### 8.8 Automatizált döntéshozatalhoz kapcsolódó jogok (GDPR 22. cikk)

Az OnWay **nem alkalmaz** automatizált egyedi döntéshozatalt és profilalkotást.

### 8.9 Panasztétel joga (GDPR 77. cikk)

A Felhasználó jogosult panaszt benyújtani a felügyeleti hatósághoz, ha úgy véli, hogy az adatkezelés sérti a GDPR rendelkezéseit.

**Magyar felügyeleti hatóság:**
> **Nemzeti Adatvédelmi és Információszabadság Hatóság (NAIH)**
> Cím: 1055 Budapest, Falk Miksa utca 9-11.
> Postai cím: 1363 Budapest, Pf. 9.
> Telefon: +36 (1) 391-1400
> E-mail: ugyfelszolgalat@naih.hu
> Honlap: https://naih.hu

## 9. A jogok gyakorlásának módja

A Felhasználó a fenti jogokat az alábbi módokon gyakorolhatja:

1. **Az Alkalmazáson belül** — a Beállítások menü megfelelő pontján (pl. „Adataim törlése")
2. **E-mailben** — a onway.help@proton.me címre küldött kéréssel

Az Adatkezelő a kéréseket legkésőbb **30 napon belül** megvizsgálja és válaszol. Bonyolult kérések esetén ez a határidő további 60 nappal meghosszabbítható.

## 10. A Tájékoztató módosítása

Az Adatkezelő fenntartja a jogot a jelen Tájékoztató egyoldalú módosítására. A módosított Tájékoztató közzétételéről és hatályba lépéséről a Felhasználót az Alkalmazásban megjelenített értesítéssel tájékoztatjuk **legalább 15 nappal** a hatálybalépés előtt.

## 11. Gyermekek védelme

Az OnWay **16. életévét betöltött** személyek számára elérhető szolgáltatás. 16 év alatti Felhasználók az Alkalmazást kizárólag a felettük szülői felügyeletet gyakorló személy hozzájárulásával használhatják, a GDPR 8. cikke, az Infotv. vonatkozó rendelkezései, valamint a Ptk. 2:13-2:14. §-ai szerint.

## 12. Elérhetőség az adatvédelmi ügyekben

- **E-mail:** onway.help@proton.me
- **Adatvédelmi tisztviselő (DPO):** Az Adatkezelő nem köteles adatvédelmi tisztviselőt kijelölni a GDPR 37. cikke alapján.

---

**Utolsó frissítés:** 2026-04-13
**Verzió:** 1.0
