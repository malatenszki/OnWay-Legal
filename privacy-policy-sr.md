# Obaveštenje o privatnosti

**Usluga:** OnWay — aplikacija za upozoravanje na saobraćajne POI
**Rukovalac podataka:** Malatenski David, fizičko lice (Srbija)
**Kontakt:** onway.help@proton.me
**Datum stupanja na snagu:** 2026-04-13
**Verzija:** 1.0

---

## 1. Rukovalac podataka

Ovo Obaveštenje o privatnosti (u daljem tekstu: **Obaveštenje**) se odnosi na lične podatke koji se obrađuju prilikom korišćenja aplikacije OnWay.

| Rukovalac | Malatenski David (fizičko lice) |
|---|---|
| Država | Srbija |
| E-mail | onway.help@proton.me |

Rukovalac obrađuje lične podatke u skladu sa **Zakonom o zaštiti podataka o ličnosti** („Sl. glasnik RS" br. 87/2018, u daljem tekstu: **ZZPL**) i **Opštom uredbom o zaštiti podataka (GDPR, Uredba (EU) 2016/679)** za Korisnike iz područja Evropske unije.

## 2. Svrha Obaveštenja

Ovo Obaveštenje ima za cilj da na transparentan način prikaže:
- koje lične podatke obrađujemo tokom pružanja Usluge
- u koju svrhu i na kom pravnom osnovu obrađujemo ove podatke
- koliko dugo čuvamo podatke
- sa kim delimo podatke
- koja prava pripadaju Korisniku u vezi sa njegovim podacima
- kako može da nas kontaktira u vezi sa obradom podataka

## 3. Kategorije ličnih podataka koje obrađujemo

Za funkcionisanje OnWay-a neophodna je obrada sledećih kategorija ličnih podataka:

### 3.1 Pseudonimni identifikator uređaja (Korisnički nalog)

- **Podaci:** Pseudonimni UUID (univerzalni jedinstveni identifikator), koji se generiše sistemom anonimne autentifikacije Supabase-a prilikom prvog pokretanja Aplikacije
- **Pravni osnov:** Član 6. stav 1. tačka (f) GDPR — **legitimni interes** Rukovaoca da pruža funkcionalnu i besplatnu POI uslugu koja zahteva razlikovanje pojedinačnih uređaja (npr. vlasništvo prijave, pravo glasanja, mere protiv zloupotreba)
- **Test ravnoteže:** Interes Korisnika za privatnost uravnotežen je sa interesom Rukovaoca da pruža i modera funkcionalnu Uslugu. Identifikator uređaja nije direktno vezan za identitet Korisnika i ne kombinuje se sa drugim izvorima u svrhu profilisanja.
- **Svrha:** Razlikovanje Korisnikovog uređaja tokom rada Usluge
- **Napomena:** Identifikator uređaja NE sadrži direktne identifikujuće podatke (bez imena, email-a, telefona) — radi se o **pseudonimnoj** obradi

### 3.2 Informacije o uređaju

- **Podaci:** Platforma (iOS / Android), verzija aplikacije, vreme poslednje aktivnosti
- **Pravni osnov:** Izvršenje ugovora + **legitimni interes** (član 6. stav 1. tačka (f) GDPR)
- **Svrha:** Pronalaženje grešaka, osiguranje kompatibilnosti platforme, obaveštenja o ažuriranjima

### 3.3 Podaci o lokaciji (GPS)

- **Podaci:** Geografska širina i dužina, smer (heading), brzina
- **Pravni osnov (u prvom planu):** Član 6. stav 1. tačka (f) GDPR — **legitimni interes** Rukovaoca da pruža POI uslugu zasnovanu na lokaciji. Dozvola operativnog sistema za lokaciju u prvom planu predstavlja efektivan mehanizam saglasnosti.
- **Pravni osnov (u pozadini):** **Izričita, zasebna in-app saglasnost** (član 6. stav 1. tačka (a) GDPR)
- **Svrha:** Centriranje mape, upozorenja u realnom vremenu o obližnjim kamerama i POI-jima
- **Čuvanje:** GPS podatke u realnom vremenu Aplikacija obrađuje **isključivo na uređaju Korisnika**, ne šalju se na server, osim ako Korisnik izričito ne pošalje prijavu (report) ili ako se evidentira događaj upozorenja

#### 3.3.1 Upravljanje saglasnošću za lokaciju u pozadini

Saglasnost za obradu lokacije u pozadini se obrađuje u skladu sa članom 7. i članom 4. stav 11. GDPR-a:

- **Davanje saglasnosti:** Lokacija u pozadini se aktivira tek nakon što Korisnik prihvati **zaseban in-app potvrdni ekran** koji jasno informiše o svrsi obrade.
- **Povlačenje saglasnosti:** Korisnik može povući saglasnost **u bilo kom trenutku, jednako jednostavno**, putem prekidača u meniju Podešavanja Aplikacije.
- **Pravno dejstvo povlačenja:** Povlačenje ne utiče na zakonitost obrade koja je ranije izvršena na osnovu saglasnosti.

### 3.4 Prijave Korisnika (Reports)

- **Podaci:** Tip prijave (policija / radar / kontrola / nezgoda), pozicija (lat/lng), smer, vreme kreiranja, vreme isteka, pseudonimni identifikator kreatora
- **Pravni osnov:** Član 6. stav 1. tačka (f) GDPR — **legitimni interes** Rukovaoca i drugih Korisnika za deljenje i primanje saobraćajnih informacija u realnom vremenu
- **Svrha:** Upozoravanje drugih Korisnika o aktuelnim uslovima na putu

### 3.5 Događaji upozorenja (Alert Events)

- **Podaci:** Izvor upozorenja (fiksna kamera ili prijava), ID izvora, vreme aktiviranja, lokacija, smer, brzina, pseudonimni identifikator upozorenog uređaja
- **Pravni osnov:** **Legitimni interes** (član 6. stav 1. tačka (f) GDPR)
- **Svrha:** Razvoj Usluge, analiza saobraćajnih obrazaca, sprečavanje zloupotreba

### 3.6 Glasovi na prijave (Report Votes)

- **Podaci:** ID prijave, pseudonimni identifikator glasača, vrednost glasa
- **Pravni osnov:** Član 6. stav 1. tačka (f) GDPR — **legitimni interes**
- **Svrha:** Zajednička moderacija prijava

### 3.7 Opcionalni nadimak

- **Podaci:** Kratko, javno ime za prikaz koje Korisnik bira u Podešavanjima
- **Pravni osnov:** Član 6. stav 1. tačka (a) GDPR — **izričita saglasnost** (polje je opcionalno)
- **Svrha:** Javna atribucija prijava i doprinosa Korisnika
- **Napomena:** Korisnik može u bilo kom trenutku obrisati ili promeniti nadimak. Rukovalac preporučuje da Korisnik ne unosi svoje stvarno ime.

### 3.8 Administratorski audit log (samo za admin korisnike)

- **Podaci:** ID administratora, izvršena radnja, ciljni objekat, vreme, IP adresa
- **Pravni osnov:** Član 6. stav 1. tačka (f) GDPR — **legitimni interes**
- **Svrha:** Praćenje administratorskih radnji

### 3.9 Šta NE obrađujemo

OnWay **izričito ne obrađuje**:
- Stvarno ime, email adresu, broj telefona (Korisnik ostaje anoniman, osim ako dobrovoljno postavi nadimak)
- Podatke o kreditnoj kartici ili plaćanju
- Profile sa društvenih mreža
- Posebne kategorije podataka
- Podatke dece (Aplikacija je za 15+, v. tačku 11)

## 4. Vreme čuvanja podataka

| Tip podatka | Vreme čuvanja |
|---|---|
| Pseudonimni red uređaja (`devices`) | Do Korisnikovog zahteva za brisanje, ili automatska anonimizacija nakon **24 meseca** neaktivnosti |
| Prijave (`reports`) | U aktivnom stanju: do isteka (45 min — 8 h). Nakon isteka: **90 dana**, zatim automatsko brisanje |
| Glasovi (`report_votes`) | Anonimizuju se kada Korisnik obriše svoj nalog; brojevi se zadržavaju bez atribucije |
| Potvrde kamera (`camera_confirmations`) | Anonimizuju se kada Korisnik obriše svoj nalog; brojevi se zadržavaju bez atribucije |
| Događaji upozorenja (`alert_events`) | **12 meseci**, zatim automatska **anonimizacija i agregirano statističko preoblikovanje** |
| Administratorski audit log (`admin_audit_log`) | **5 godina** |
| GPS podaci (u realnom vremenu) | **NE ČUVAJU SE** na serveru |

## 5. Obrađivači podataka i prosleđivanje trećim licima

Za pružanje Usluge Rukovalac koristi sledeće obrađivače podataka:

### 5.1 Glavni obrađivač: Supabase

- **Naziv:** Supabase Inc.
- **Uloga:** Baza podataka, autentifikacija, cloud backend usluga
- **Lokacija čuvanja:** **AWS eu-west-3 region — Pariz, Francuska** (teritorija EU)
- **Pravni osnov:** Ugovor o obradi podataka (DPA) prema članu 28. GDPR-a
- **Više informacija:** https://supabase.com/privacy

### 5.2 Pružalac mapovskih pločica: OpenStreetMap

- **Naziv:** OpenStreetMap Foundation (OSMF)
- **Uloga:** Isporuka mapovskih pločica
- **Lokacija:** Serveri na teritoriji Evropske unije
- **Više informacija:** https://osmfoundation.org/wiki/Privacy_Policy

### 5.3 Pružaoci platforme (mobile store)

- **Apple Inc.** (App Store) — SAD, na osnovu EU-US Data Privacy Framework
- **Google LLC** (Google Play Store) — SAD, na osnovu EU-US Data Privacy Framework

### 5.4 Push notifikacije (buduća funkcija)

Ako Aplikacija uvede push notifikacije, push token i sadržaj će se preneti putem APNs ili FCM. **Trenutno nije aktivno.**

### 5.5 Ne prodajemo podatke

Rukovalac **ne prodaje, ne iznajmljuje i ne prosleđuje u marketinške svrhe** lične podatke Korisnika trećim licima.

## 6. Međunarodni prenos podataka

Rukovalac primarno čuva podatke **na teritoriji Evropske unije**. Za obrađivače van EU prenos se vrši na osnovu:

- **EU-US Data Privacy Framework** (sprovedbena odluka Evropske komisije 2023/1795)
- **Standard Contractual Clauses (SCC)** — odluka 2021/914
- Po potrebi, dodatne tehničke i organizacione mere

## 7. Mere bezbednosti

Rukovalac primenjuje:

- **Enkriptovan prenos podataka** (HTTPS/TLS 1.2+)
- **Enkriptovano čuvanje** (AES-256 at-rest)
- **Row Level Security (RLS)** na nivou baze
- **Pseudonimizacija** identifikacije Korisnika
- **Administratorski audit log**
- **Dvofaktorska autentifikacija (2FA)** za administratorski pristup
- **Automatski backup** svakodnevno

## 8. Prava Korisnika

Prema GDPR-u i ZZPL-u, Korisniku pripadaju sledeća prava:

### 8.1 Pravo na pristup (član 15. GDPR / član 26. ZZPL)
Korisnik ima pravo da traži informaciju o tome da li obrađujemo njegove podatke.

### 8.2 Pravo na ispravku (član 16. GDPR / član 29. ZZPL)
Korisnik ima pravo da traži ispravku netačnih podataka.

### 8.3 Pravo na brisanje (član 17. GDPR / član 30. ZZPL)
Korisnik može u bilo kom trenutku zahtevati brisanje. To je dostupno i unutar Aplikacije kroz **„Obriši moje podatke"** opciju (Podešavanja → Privatnost) ili e-mailom.

### 8.4 Pravo na ograničenje obrade (član 18. GDPR / član 31. ZZPL)
Korisnik može da zahteva ograničenje obrade pod određenim uslovima.

### 8.5 Pravo na prenosivost podataka (član 20. GDPR / član 36. ZZPL)
Korisnik ima pravo da dobije svoje podatke u **mašinski čitljivom formatu** (JSON).

### 8.6 Pravo na protivljenje (član 21. GDPR / član 37. ZZPL)
Korisnik može da se protivi obradi zasnovanoj na legitimnom interesu.

### 8.7 Pravo na povlačenje saglasnosti (član 7. stav 3. GDPR)
Saglasnost može da se **u bilo kom trenutku besplatno povuče**.

### 8.8 Automatizovano donošenje odluka (član 22. GDPR)
OnWay **ne primenjuje** automatizovano pojedinačno odlučivanje ili profilisanje.

### 8.9 Pravo na pritužbu (član 77. GDPR / član 82. ZZPL)

**Srpski nadzorni organ:**
> **Poverenik za informacije od javnog značaja i zaštitu podataka o ličnosti**
> Bulevar kralja Aleksandra 15, 11000 Beograd
> Telefon: +381 11 3408 900
> E-mail: office@poverenik.rs
> Web: https://www.poverenik.rs

## 9. Način ostvarivanja prava

1. **Unutar Aplikacije** — kroz odgovarajuće opcije u meniju Podešavanja
2. **E-mail-om** — zahtevom poslatim na onway.help@proton.me

Rukovalac razmatra zahteve u roku od **30 dana**.

## 10. Izmena ovog Obaveštenja

Rukovalac zadržava pravo na jednostranu izmenu. Korisnik će biti obavešten najmanje **15 dana** pre stupanja na snagu.

## 11. Zaštita dece

OnWay je usluga dostupna licima **koja su napunila 15 godina**, u skladu sa **članom 16. Zakona o zaštiti podataka o ličnosti** Republike Srbije. Lica mlađa od 15 godina mogu koristiti Aplikaciju samo uz saglasnost roditelja.

## 12. Kontakt za pitanja o privatnosti

- **E-mail:** onway.help@proton.me
- **Službenik za zaštitu podataka (DPO):** Rukovalac nije obavezan da imenuje DPO u skladu sa članom 37. GDPR.

---

**Poslednje ažuriranje:** 2026-04-13
**Verzija:** 1.0
