# familedashboard
Felles kalender for vår familie
# 🏠 Familiedashboard – Prosjektplan

Et kontekstsensitivt familiedashboard for Marcus, Ragnhild, Alvar (12), Ovidia (8) og Edvald (5).
Inspirert av Tesla-skjermens filosofi: vis kun det som er relevant akkurat nå.

**Live URL:** https://marcussteinsvaag-beep.github.io/familedashboard

---

## ✅ Ferdig bygget

### Grunnmur
- Klokke og dato med norsk formatering
- Mørkt skandinavisk design (DM Serif + DM Sans)
- Responsivt layout for laptop og iPad
- GitHub Pages-hosting

### Vær – Yr.no
- Sanntidsvær med temperatur, vind, nedbør og føles-som
- 5-dagers prognose
- **Stedssensitivt vær** – bytter automatisk basert på kalenderoppføringer:
  - Standard: Haslum (59.9181, 10.5311)
  - Tjøme (59.1167, 10.4167) – trigger: "tjøme", "sommerhytt"
  - Elgåsen (60.8580, 10.8450) – trigger: "elgåsen", "sjusjøen", "fjellhytt"
  - Fåvangfjellet (61.4560, 10.2210) – trigger: "fåvang", "sportskapell"

### Google Kalender
- 7 dager frem med fargekoding
- Viser tid, tittel og sted per hendelse
- Spond-hendelser kommer automatisk via Google Kalender-integrasjon
- Datoberegning i lokal tid (UTC+2 bug fikset)

### Bursdagsvarsler
- Egen liste uavhengig av Google Kalender
- Varsler 3, 2 og 1 dag i forveien + selve dagen
- Viser korrekt alder basert på fødselsår
- Nåværende liste: Farmor Linda, Farfar Johnny, Alvar, Ovidia, Edvald

### Hvem er hvor
- Statusrad for alle 5 familiemedlemmer
- Klikk for å sykle gjennom statuser: 🏠 🏢 ⚽ 🏥 🛒 ✈️ 🌊 ⛷️
- Lagres lokalt i nettleseren

### Ukens middag
- 7-dagers ukesvisning med emoji basert på matnavn
- Klikk for å redigere hvilken dag som helst
- 👍/👎 stemming for barna
- Lagres lokalt

### Handleliste
- Enkel delt liste
- Legg til varer, huk av når kjøpt
- Lagres lokalt

### Nattmodus (22:00–06:00)
- Skjermen dimmes automatisk
- Trykk hvor som helst for å vekke i 2 minutter
- Vekkeknapp nederst på skjermen

### Kontekstsensitiv visning
- **Morgen (06–09, man–fre):** Kjøretid til jobb vises
- **Kveld (19:30+):** Kveldsrutine med nedtelling vises
- **Hverdagskvelder (20–23):** Kveldsjekkliste vises
- **Helg:** Kveldsrutine justeres til helgevariant

### Kjøretid til jobb (man–fre 06–09)
- Rute: Vestliveien 20B → Haslum skole → Innspurten 15
- Sanntidstrafikk via Google Directions API
- Fargekoding: grønn/gul/rød basert på forsinkelse
- Vises IKKE i helger

### Kveldsrutine (hverdager)
- 19:30 – Kveldsmat
- 20:00 – Edvald: bad og tannpuss
- 20:15 – Edvald: legging
- 20:30 – Ovidia: tannpuss
- 21:00 – Ovidia: legging
- 21:30 – Alvar: skjermfri tid
- 22:00 – Alvar: legging
- 22:00 – Voksne: ro og fred 🍷
- Nedtelling per punkt (grønn → gul → rød)
- Helgevariant med senere tider

### Kveldsjekkliste (hverdagskvelder)
- Tøm oppvaskmaskinen
- Matboks til Alvar og Ovidia
- Vannflasker x3
- Dynamisk: legger til treningsbag/instrument hvis aktivitet neste dag
- Nullstilles automatisk neste dag

### Morgenrutine-påminnelser (06–09, man–fre)
- Kombinerer kalender + vær
- Eksempel: "⚽ Husk fotballutstyr til Alvar" når trening er i kalenderen
- "☂️ Regnjakke til barna" når det varsles regn
- "🧤 Votter og lue" når under 2 grader

### Prosjektkort
- Knapp på kalenderoppføringer som matcher hytte-steder
- Åpner modal med sjekkliste og handleliste
- ⛵ Båtpuss Tjøme
- ⛷️ Åpning fjellhytta Elgåsen
- 🏔️ Fåvangfjellet sportskapell
- Husker avhukinger mellom besøk, kan nullstilles

### Bortekamp-varsling
- Oppdager "borte" eller "bortekamp" i kalenderoppføringer med sted
- Henter kjøretid via Directions API
- Beregner anbefalt avreisetid (kampstart - kjøretid - 20 min buffer)
- Viser: "🚗 Anbefaler avreise kl 16.15 (34 min kjøring + 20 min buffer)"

### Ferienedtelling
- Finner første kommende hytte-oppføring i kalender
- Viser antall dager til Tjøme, Elgåsen eller Fåvangfjellet

---

## 🔄 Planlagt – ikke bygget ennå

### Familiebanken (høy prioritet)
Poengsystem for barna som motiverer til husarbeid.

**Oppgaver og poeng:**
- Søppel ut: 5p
- Tømme oppvaskmaskin: 5p
- Dekke bordet: 3p
- Rydde rommet: 8p
- Støvsuge: 10p
- Hjelpe med matlaging: 8p
- Vaske bad: 12p
- Handle: 10p
- Mate akvariefiskene: 3p (kun én per dag – Ovidia og Edvald konkurrerer)
- Alvar: hente søsken: 15p
- Alvar: lage middag: 20p

**Belønninger (veksles inn – poeng trekkes fra):**
- 50p: Velge kveldsfilm 🎬
- 100p: Is eller godteri-kveld 🍦
- 150p: Velge fredagsmiddag 🌮
- 200p: Venn på overnatting 🏕️
- 300p: Valgfri aktivitet (kino, bowling etc) 🎳

**Viktige detaljer:**
- Alle tre barna deltar (Edvald får enkle oppgaver)
- Barna registrerer selv – tillitsbasert
- Admin-panel for voksne til å korrigere/gi bonus
- Poeng akkumuleres og veksles inn (nullstilles ikke ukentlig)
- Historikk per barn
- Fremgangsbar mot neste belønning

### Ukeplaner med AI-lesing (høy prioritet)
- Søndagspåminnelse: "Last opp ukeplaner for alle tre"
- Opplasting av PDF/Word for Alvar og Ovidia (samme format, Alvar bytter til ungdomsskole august 2026)
- Skjermbilde av barnehageapp for Edvald
- AI leser dokumentene og trekker ut lekser/aktiviteter per dag
- Viser dagens lekser tydelig på dashboardet

**Edvalds faste barnehagerytme:**
- Mandag: 🎒 Ha-med-dag
- Onsdag: 🥾 Turdag – ekstra matpakke
- Fredag (fra medio april): 🚲 Sykkeldag – husk hjelm
- Barnehagen har også ukentlig varierende aktiviteter (skjermbilde)

### Designrunde (høy prioritet)
- Skikkelig portrait-optimalisering for iPad
- Bedre typografisk hierarki
- Mer luft og romfølelse
- Fargekoding per person i kalender (ikke tilfeldig)
- Animasjoner og micro-interactions
- Kontekstsensitiv fargetemperatur (varmere om kvelden)

### Tekniske forbedringer
- Cloudflare Worker proxy for API-nøkler (som Growatt-løsningen)
- Firebase for sanntidsdeling av handleliste og middagsplan mellom enheter
- GitHub Pages er nok for nå

---

## 📱 Oppsett

**Enheter:**
- iPad Pro på kjøkkenet (primær visningsenhet)
- Tilgjengelig fra alle enheter via GitHub Pages URL

**Teknologi:**
- Ren HTML/CSS/JavaScript – ingen rammeverk
- Google Calendar API
- Google Directions API
- Yr.no locationforecast API (gratis, ingen nøkkel)
- localStorage for midlertidig datalagring

**Konfigurasjon i index.html:**
- `GOOGLE_API_KEY` – begrenset til Calendar og Directions API, kun fra github.io-domenet
- `CALENDAR_ID` – familiekalenderen (j6icirppgh0fdeb3f9s6p3pfng@group.calendar.google.com)
- `BIRTHDAYS` – familiens bursdager med navn, dato, fødselsår og emoji
- `LOCATIONS` – koordinater for alle steder
- `ROUTINES_WEEKDAY` / `ROUTINES_WEEKEND` – kveldsrutiner

---

## 💡 Fremtidige ideer (ikke besluttet)

- Oda-varsling når leveringsbil nærmer seg (via Tasker på Android)
- Tibber strømpris-visning
- Skolerute-teller ("X dager til sommerferien")
- Søvnvennlig progressiv dimming fra 21:00
- Familiemål/motivasjonsquote
- Kommersielt potensial: abonnementsbasert familieplatform for travle familier

---

## 🗓️ Historikk

- **13. april 2026:** Første versjon live på GitHub Pages
  - Kalender, vær, nattmodus, bursdager, kjøretid, kveldsrutine fungerer
  - UTC/lokal tid-bug fikset
  - API-nøkkel begrenset til github.io-domenet

---

*Neste arbeidsøkt: Familiebanken og ukeplaner*
