# Onderwijskundige Review & Verbeterplan Les 1
## Time Series Data & Preprocessing

**Datum review:** 5 december 2025
**Reviewer perspectief:** Formatief handelen, Directe instructie, Modern effectief HBO onderwijs

---

## EXECUTIVE SUMMARY

**Algemene beoordeling:** 5.7/10

De les heeft een solide structuur met goede hands-on activiteiten, maar mist essentiële elementen voor effectief HBO onderwijs:
- Formatief handelen gebeurt te laat en te weinig systematisch
- Directe instructie mist expliciete modeling en guided practice
- Transfer naar beroepspraktijk en hogere-orde denken zijn onderontwikkeld

**Prioriteit verbeteringen:**
1. 🔴 HIGH: Voeg formatieve checks toe TIJDENS de les
2. 🔴 HIGH: Implementeer expliciete "I do, We do, You do" structuur
3. 🟡 MEDIUM: Versterk link naar beroepspraktijk met authentieke cases
4. 🟡 MEDIUM: Voeg worked examples toe in notebook
5. 🟢 LOW: Verbeter reflectiemomenten met metacognitieve prompts

---

## GEDETAILLEERDE ANALYSE

### 1. FORMATIEF HANDELEN (Score: 5/10)

#### ✅ Wat werkt goed:
- **Exit ticket**: Duidelijke vragen aan het einde
- **Think-Pair-Share**: Activerende didactiek
- **Peer review**: Studenten leren van elkaar
- **Observatie**: Docent loopt rond tijdens hands-on

#### ❌ Wat moet beter:

**Probleem 1: Te weinig tussentijdse checks**
- Exit ticket komt pas na 120 minuten - te laat om bij te sturen
- Geen checks na mini-lectures of studenten het begrijpen
- Studenten werken door zonder te weten of ze op de goede weg zijn

**Probleem 2: Geen succescriteria**
- Studenten weten niet wat "goed genoeg" is
- Reflectievragen zijn te open zonder criteria
- Geen rubrics of checklists

**Probleem 3: Feedback ontbreekt**
- Peer review heeft geen structuur/criteria
- Geen moment waarop docent systematisch feedback geeft
- Exit ticket wordt niet besproken met studenten

**Probleem 4: Self-assessment ontbreekt**
- Studenten kunnen hun eigen begrip niet monitoren
- Geen traffic light momenten ("rood/oranje/groen")
- Geen self-check vragen in notebook

#### 🔧 CONCRETE VERBETERINGEN:

**Verbetering 1A: Voeg "Check for Understanding" momenten toe**

**Na elke mini-lecture** (3x in de les):
```
MINI POLL (1-2 min):
- Toon multiple choice vraag op scherm
- Studenten stemmen (hand opsteken / Mentimeter / kleuren kaartjes)
- Bij <70% goed: herhaal kernpunt met ander voorbeeld
- Bij >70% goed: ga door

Voorbeeld na Blok 1:
"Welke is een time series?
A) DNA sequentie
B) Hartslag per seconde ✓
C) Woorden in een zin
D) Producten in winkelmandje"
```

**Verbetering 1B: Traffic Light Check (3x in de les)**

Na elk blok:
```
TRAFFIC LIGHT (1 min):
Studenten tonen kleur:
🟢 Groen: "Ik begrijp het en kan het uitleggen"
🟡 Oranje: "Ik begrijp het grotendeels maar heb vragen"
🔴 Rood: "Ik ben de draad kwijt"

Actie:
- Bij veel rood/oranje: plenum uitleg
- Bij weinig rood/oranje: individuele support tijdens werk
```

**Verbetering 1C: Succescriteria zichtbaar maken**

Aan het begin van elk blok:
```
SUCCES CRITERIA CHECKLIST:

Blok 2 - Karakteristieken:
□ Ik kan trend, seasonality en noise identificeren in een grafiek
□ Ik kan uitleggen waarom stationariteit belangrijk is
□ Ik kan een stationaire en niet-stationaire series van elkaar onderscheiden

→ Deze checklist komt op het scherm EN in het notebook
→ Studenten vinken af bij peer review
```

**Verbetering 1D: Notebook Self-Checks**

Voeg toe na elke techniek in het notebook:
```python
# ✅ SELF-CHECK
# Voordat je verder gaat, controleer:
# 1. Snap je waarom we interpolatie gebruiken? (Ja/Nee/Beetje)
# 2. Kun je uitleggen wanneer je forward fill vs interpolatie gebruikt?
# 3. Draai de code en begrijp je de output?
#
# Nog niet zeker? Vraag je buurpersoon of docent!
```

**Verbetering 1E: Gestructureerde Peer Review**

Vervang "Wissel notebooks" met:
```
PEER REVIEW PROTOCOL (5 min):

Stap 1: Wissel notebooks
Stap 2: Check aan de hand van criteria:
  ✓ Zijn alle cells uitgevoerd?
  ✓ Zijn grafieken leesbaar met labels?
  ✓ Is de gekozen window size/alpha gedocumenteerd?
  ✓ Staan er observaties bij experimenten?

Stap 3: Geef 1 compliment en 1 tip
Stap 4: Bespreek samen: welke aanpak werkt beter en waarom?
```

---

### 2. DIRECTE INSTRUCTIE (Score: 6/10)

#### ✅ Wat werkt goed:
- **Duidelijke leerdoelen** (LO6 en LO7)
- **Logische opbouw** van basis naar complex
- **Concrete voorbeelden** (temperatuur, sensoren)
- **Stapsgewijze workshop** met 4 technieken

#### ❌ Wat moet beter:

**Probleem 1: Geen expliciete "I do, We do, You do"**
- Studenten beginnen direct met opdrachten zonder modeling
- Docent demonstreert niet eerst HOE je iets doet
- Te snel van instructie naar zelfstandig werk

**Probleem 2: Ontbrekende worked examples**
- In notebook krijgen studenten code zonder uitleg
- Geen stap-voor-stap uitleg van redenering
- Studenten moeten zelf uitvogelen hoe code werkt

**Probleem 3: Mini-lectures te kort**
- 10 minuten is te weinig voor modeling + uitleg + voorbeelden
- Te veel informatie in te korte tijd

**Probleem 4: Geen checking tussen stappen**
- Van mini-lecture direct naar groepsopdracht zonder check
- Van uitleg naar zelfstandig werk zonder guided practice

#### 🔧 CONCRETE VERBETERINGEN:

**Verbetering 2A: Implementeer "I do, We do, You do" structuur**

**BLOK 1: Time Series vs Sequential Data**

Huidige structuur (SLECHT):
```
Mini-lecture (10 min) → Groepsopdracht (15 min)
```

Nieuwe structuur (GOED):
```
I DO (7 min):
- Docent toont 2 voorbeelden
- Denkt hardop: "Dit is time series omdat... Ik zie dat..."
- Demonstreert categorisatie proces

WE DO (8 min):
- Docent toont nieuw voorbeeld
- Studenten roepen mee: "Is dit time series? Waarom?"
- Plenum: discussie met docent als gids
- Check for understanding poll

YOU DO (10 min):
- Groepsopdracht zoals nu
- Docent loopt rond en ondersteunt
```

**Verbetering 2B: Voeg worked examples toe aan notebook**

Voeg toe VOOR elke techniek:
```python
# ==========================================
# 📖 WORKED EXAMPLE: Missing Data
# ==========================================
#
# Probleem: We hebben sensor data met missing values op tijdstip 5, 6, 7
# Data: [10, 12, 14, 16, NaN, NaN, NaN, 28, 30]
#
# Stap 1: Bekijk de situatie
#   - 3 opeenvolgende missing values
#   - Er is een duidelijke trend (stijgend)
#
# Stap 2: Overwegen opties
#   - Forward fill: zou 16, 16, 16 geven → ignoreert stijgende trend ❌
#   - Backward fill: zou 28, 28, 28 geven → grote sprong ❌
#   - Linear interpolation: zou 18, 20, 22, 24, 26 geven → volgt trend ✓
#
# Stap 3: Keuze
#   Voor deze situatie is LINEAR INTERPOLATION het beste
#   Waarom? Het respecteert de onderliggende trend
#
# Stap 4: Code
data = pd.Series([10, 12, 14, 16, np.nan, np.nan, np.nan, 28, 30])
filled_data = data.interpolate(method='linear')
print(filled_data)
# Output: [10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30]

# ✅ Zie je hoe de waarden mooi oplopen van 16 naar 28?
# ==========================================

# 👉 NU JIJ: Pas deze techniek toe op de energy data hieronder:
```

**Verbetering 2C: Uitbreiden mini-lectures**

**Van:**
```
Mini-lecture (10 min): Definitie + voorbeelden
```

**Naar:**
```
MINI-LECTURE (15 min):

1. Activatie (2 min): "Wat weet je al?"
2. Kernbegrippen (5 min): Definitie met visuele ondersteuning
3. Modeling (5 min): Docent demonstreert met denk-hardop
4. Check (2 min): Quick poll
5. Samenvatten (1 min): Studenten zeggen kernpunten
```

**Verbetering 2D: Guided Practice toevoegen**

Voor blok 3 (Transformatie Technieken):

**Huidige structuur:**
```
Probleemstelling (5 min) → Hands-on workshop (25 min)
```

**Nieuwe structuur:**
```
Probleemstelling (5 min)
↓
GUIDED PRACTICE (10 min):
- Docent doet EERSTE techniek (missing data) live
- Studenten kijken mee en maken aantekeningen
- Docent stelt vragen: "Wat denk je dat er nu gebeurt?"
- Code wordt stap-voor-stap uitgelegd
↓
SCAFFOLDED PRACTICE (20 min):
- Studenten doen technieken 2, 3, 4 zelfstandig
- Met decreasing support (meer hints bij 2, minder bij 4)
↓
INDEPENDENT PRACTICE (5 min):
- Studenten kiezen parameters en experimenteren
```

**Verbetering 2E: Beslisboom voor praktijk**

Voeg toe aan het einde van elk blok:
```python
# 🧭 DECISION GUIDE: When to use what?

# MISSING DATA:
# Use forward fill when: → Recent value is best predictor (slowly changing data)
# Use interpolation when: → There's a clear trend/pattern
# Use backward fill when: → Future value is more relevant than past
# Use mean when: → You have no better information

# YOUR RULE OF THUMB:
# For sensor/time series data → INTERPOLATION is usually best ✓
```

---

### 3. MODERN EFFECTIEF HBO ONDERWIJS (Score: 6/10)

#### ✅ Wat werkt goed:
- **Authentieke tools** (Python, Pandas - industrie standaard)
- **Hands-on learning** (veel praktijk)
- **Collaborative learning** (groepswerk, peer review)
- **Echte data** (energieverbruik)

#### ❌ Wat moet beter:

**Probleem 1: Zwakke link naar beroepspraktijk**
- Energieverbruik voorbeeld is abstract
- Geen expliciete connectie met HBO beroepen
- Ontbreekt: "Waarom is dit relevant voor mij als HBO'er?"

**Probleem 2: Blijft steken in "toepassen"**
- Bloom: studenten passen toe, maar analyseren/evalueren/creëren ontbreekt
- Weinig kritisch denken: "Welke techniek is BETER en waarom?"
- Geen complexe beslissingen

**Probleem 3: Transfer ontbreekt**
- Studenten werken alleen met gegeven data
- Geen moment: "Hoe pas je dit toe in je eigen project/stage?"
- Geen generalisatie naar andere contexten

**Probleem 4: Oppervlakkige reflectie**
- Reflectievragen zijn descriptief, niet metacognitief
- Exit ticket meet recall, niet begrip/transfer

**Probleem 5: Differentiatie niet uitgewerkt**
- Alleen vermeld in algemene tips
- Geen concrete differentiatie in opdrachten

#### 🔧 CONCRETE VERBETERINGEN:

**Verbetering 3A: Authentieke beroepspraktijk case**

Vervang abstract "energieverbruik" met een van deze cases:

**Optie 1: Healthcare (Verpleegkunde/Fysiotherapie):**
```
CASE: JIJ BENT DATA ANALIST BIJ ZIEKENHUIS RIJNSTATE

Probleem:
- Hartslag monitoring patiënten heeft vaak missing values (sensor losgeraakt)
- Er zijn outliers (patiënt bewoog, artefacten)
- Data is noisy (ademhaling beïnvloedt hartslag)

Jouw taak:
- Maak de data geschikt voor Early Warning Score systeem
- Verkeerde preprocessing = gemiste waarschuwingen = gevaar!

Wat zijn de consequenties als je:
- Missing values verkeerd invult?
- Outliers niet detecteert?
- Te veel smoothing toepast?
```

**Optie 2: Business/Marketing:**
```
CASE: JIJ BENT DATA SCIENTIST BIJ BOL.COM

Probleem:
- Dagelijkse verkoopcijfers voor voorraad planning
- Black Friday zorgt voor extreme outliers
- Corona periode heeft trend verstoord
- Sommige dagen geen data (systeem downtime)

Jouw taak:
- Voorspel volgende week verkoop
- Maar eerst: clean de historische data
- Verkeerde keuze = te veel of te weinig voorraad = miljoenen verlies
```

**In opening van les:**
```
"Jullie zijn niet hier om Python te leren.
Jullie zijn hier om BESLISSINGEN TE NEMEN met data.
In je toekomstige baan ga je dit ELKE DAG doen.

Vandaag leer je: Hoe maak ik data betrouwbaar genoeg
om er business/healthcare/engineering beslissingen op te baseren?"
```

**Verbetering 3B: Hogere-orde denken opdrachten**

Voeg EVALUATIE en CREATIE opdrachten toe:

**Na Blok 2 (in plaats van simpele Think-Pair-Share):**
```
CASE ANALYSE (10 min):

Je krijgt 3 verschillende time series:
1. Hartslag patient (per seconde)
2. Website verkeer (per uur)
3. Jaarlijkse temperatuur (per dag)

Voor elk:
□ Welke component (trend/seasonality/noise) is dominant?
□ Waarom is dit belangrijk voor analyse?
□ Welke preprocessing heeft hoogste prioriteit?
□ Wat zijn de RISICO'S van verkeerde preprocessing?

→ Dit is EVALUEREN op Bloom taxonomie
```

**Na Blok 3 (in plaats van simpele experimenten):**
```
DESIGN CHALLENGE (15 min):

Gegeven: Temperatuur data van productiehal met:
- Missing: 5%
- Outliers: Machine restart zorgt voor spikes
- Noise: Veel
- Doel: Detecteer overhitting (>30°C) voor alarm systeem

Design je preprocessing pipeline:
1. Welke technieken gebruik je?
2. In welke VOLGORDE? (Waarom?)
3. Welke parameters kies je? (Waarom?)
4. Wat zijn de TRADE-OFFS van je keuzes?
5. Hoe TEST je of je pipeline goed werkt?

→ Dit is CREËREN op Bloom taxonomie
```

**Verbetering 3C: Transfer naar eigen context**

**Voeg toe voor afsluiting:**
```
TRANSFER OEFENING (10 min):

Individueel (5 min):
- Denk aan je afstudeerstage of minor project
- Welke time series data zou je daar tegen kunnen komen?
- Schrijf op:
  * Jouw data: _________
  * Welke preprocessing problemen verwacht je?
  * Welke 2 technieken uit vandaag ga je zeker gebruiken?

Pair-Share (5 min):
- Deel met buurpersoon
- Help elkaar: "Voor jouw data zou ik... omdat..."

→ Dit zorgt voor TRANSFER naar eigen praktijk
```

**Verbetering 3D: Metacognitieve reflectie**

Vervang exit ticket met diepere reflectie:

**Huidige exit ticket (TE OPPERVLAKKIG):**
```
1. Noem één verschil tussen time series en sequential data
2. Welke techniek voor ruis?
3. Eén vraag
```

**Nieuwe exit ticket (METACOGNITIEF):**
```
EXIT REFLECTION (5 min):

1. BEGRIP:
   Wat was het moeilijkste concept vandaag?
   Waarom was het moeilijk voor jou?

2. STRATEGIE:
   Welke strategie heb je gebruikt om het toch te begrijpen?
   (Voorbeelden bekijken / met medestudent praten / code draaien / ...)

3. TOEPASSING:
   Beschrijf één situatie in je toekomstige beroep waar je
   time series preprocessing gaat gebruiken.
   Welke techniek zou je toepassen? Waarom?

4. VERBINDING:
   Hoe verbindt dit met wat je al wist uit andere vakken?
   (Statistiek / Programmeren / Wiskunde / ...)

5. NEXT STEP:
   Wat wil je nog oefenen voor je dit echt beheerst?
```

**Verbeering 3E: Uitgewerkte differentiatie**

**Voor snelle studenten - VERRIJKING (in notebook):**
```python
# ⭐ CHALLENGE for fast finishers:
#
# Research question: Does the ORDER of preprocessing steps matter?
#
# Experiment:
# Pipeline A: Remove outliers → Smooth → Normalize
# Pipeline B: Smooth → Remove outliers → Normalize
#
# 1. Implement both pipelines
# 2. Compare results visually
# 3. Which is better? Why?
# 4. Formulate a RULE for correct order
#
# Bonus: Find academic paper about preprocessing pipelines
```

**Voor langzame studenten - SCAFFOLDING:**
```python
# 🆘 NEED HELP? Use this guided version:

# Step 1: Fill in the missing parameter
data_cleaned = data.interpolate(method='___')  # Hint: we want linear

# Step 2: Run this cell and check: does the line look smooth? (Yes/No)

# Step 3: If No, try method='___' instead  # Options: 'linear', 'quadratic'

# Step 4: Ask your neighbor: which method did you choose? Why?
```

**Voor verschillende niveaus - KEUZE:**
```
Blok 3 hands-on workshop:

NIVEAU KEUZE:
□ Level 1: Follow guided notebook (all code provided, fill in gaps)
□ Level 2: Semi-guided (function signatures provided, implement logic)
□ Level 3: Challenge (only requirements, write all code yourself)

→ Studenten kiezen zelf niveau op basis van self-assessment
```

---

## IMPLEMENTATIE PRIORITEITEN

### 🔴 CRITICAL - Implementeer NU (anders leerdoelen niet gehaald):

1. **Formatieve checks tijdens les** (Verbetering 1A, 1B)
   - Zonder dit weet je niet of studenten meekomen
   - Implementatie: 30 min voorbereiden (polls maken)

2. **"I do, We do, You do" structuur** (Verbetering 2A)
   - Zonder modeling snappen studenten niet HOE
   - Implementatie: 1 uur lesplan herstructureren

3. **Worked examples in notebook** (Verbetering 2B)
   - Zonder dit kunnen studenten niet zelfstandig leren
   - Implementatie: 2 uur notebook aanpassen

### 🟡 IMPORTANT - Implementeer deze maand:

4. **Authentieke beroepspraktijk case** (Verbetering 3A)
   - Verhoogt motivatie en relevantie enorm
   - Implementatie: 1 uur case schrijven

5. **Succescriteria zichtbaar** (Verbetering 1C)
   - Studenten weten nu niet wat "goed genoeg" is
   - Implementatie: 30 min criteria formuleren

6. **Hogere-orde denken opdrachten** (Verbetering 3B)
   - HBO niveau vereist analyse en evaluatie
   - Implementatie: 1 uur opdrachten ontwerpen

### 🟢 NICE TO HAVE - Plan voor volgend semester:

7. **Metacognitieve reflectie** (Verbetering 3D)
   - Verbetert leren op lange termijn
   - Implementatie: 30 min nieuwe exit ticket

8. **Uitgewerkte differentiatie** (Verbetering 3E)
   - Helpt alle studenten op hun niveau
   - Implementatie: 1-2 uur niveaus uitwerken

9. **Transfer oefening** (Verbetering 3C)
   - Verbindt met eigen praktijk
   - Implementatie: 30 min opdracht schrijven

---

## CONCRETE ACTIEPLAN

### Week 1 (4 uur werk):
- [ ] Maak 3 "Check for Understanding" polls (Mentimeter / Kahoot)
- [ ] Herstructureer Blok 1 en 2 naar "I do, We do, You do"
- [ ] Schrijf 1 worked example voor missing data techniek

### Week 2 (4 uur werk):
- [ ] Schrijf 3 extra worked examples (noise, normalization, outliers)
- [ ] Pas notebook aan met worked examples
- [ ] Test notebook met collega

### Week 3 (3 uur werk):
- [ ] Kies en uitwerk 1 authentieke beroepspraktijk case
- [ ] Maak succescriteria checklist per blok
- [ ] Ontwerp Traffic Light check instructie

### Week 4 (2 uur werk):
- [ ] Ontwerp 2 hogere-orde opdrachten (evaluatie + creatie)
- [ ] Implementeer in lesplan
- [ ] Test gehele les met collega (dry-run)

**Totale tijdsinvestering: 13 uur** (over 4 weken)
**Verwachte verbetering: 5.7/10 → 8.5/10**

---

## VOORBEELD UITWERKING: Blok 1 met alle verbeteringen

Hier is een volledig uitgewerkte versie van Blok 1 met alle verbeteringen geïmplementeerd:

### **Blok 1: Time Series vs Sequential Data (30 min)**

#### **Opening: Succescriteria zichtbaar maken (2 min)**

```
Docent toont op scherm:

🎯 AAN HET EINDE VAN DIT BLOK KUN JIJ:
□ Uitleggen wat time series data is (met eigen woorden)
□ Het verschil uitleggen tussen time series en sequential data
□ Nieuwe voorbeelden correct categoriseren
□ Uitleggen WAAROM dit onderscheid belangrijk is in je beroep

✅ Check deze lijst aan het einde van het blok!
```

#### **I DO: Modeling (7 min)**

```
Docent: "Ik ga jullie laten ZIEN hoe ik dit analyseer. Let op mijn redenering."

[Toont slide met 2 voorbeelden]

Voorbeeld 1: Hartslag gemeten elke seconde gedurende hardlopen
Voorbeeld 2: DNA sequentie van een virus

Docent denkt HARDOP:
"Oké, eerst kijk ik naar voorbeeld 1 - hartslag data.
Ik vraag mezelf af: Is TIJD belangrijk hier?
Ja! Want als mijn hartslag nu 180 is en over 10 seconden 120,
dan is dat belangrijk - ik ben aan het afkoelen.
Als ik de volgorde verander, verlies ik die informatie.

En zijn de intervallen regelmatig?
Ja! Elke seconde een meting. 1, 2, 3, 4...

Conclusie: Dit is TIME SERIES data. ✓

Nu voorbeeld 2 - DNA sequentie: ATGCCGTA
Vraag: Is tijd belangrijk?
Nee! Het gaat om de VOLGORDE van letters, niet wanneer ze zijn geobserveerd.
Is interval belangrijk?
Nee! Er is geen 'tijd tussen letters'.

Conclusie: Dit is SEQUENTIAL data. ✓

Zie je het verschil? Bij TIME SERIES is WANNEER cruciaal,
bij SEQUENTIAL is VOLGORDE cruciaal maar WANNEER niet."

[Check for Understanding]
```

#### **CHECK FOR UNDERSTANDING: Quick Poll (2 min)**

```
Docent: "Nu ga ik checken of je het snapt."

[Toont Mentimeter poll]

Vraag: Welke van deze is TIME SERIES data?

A) Woorden in een zin
B) Dagelijkse temperatuur over een jaar ✓
C) DNA sequentie
D) Producten in je Netflix kijkgeschiedenis

Studenten stemmen → Resultaten direct zichtbaar

Als <70% goed:
"Ik zie dat veel mensen A of D kozen. Laat ik het opnieuw uitleggen..."
[Herhaal kernpunt met nieuw voorbeeld]

Als >70% goed:
"Top! Jullie snappen het. Laten we samen één voorbeeld doen."
```

#### **WE DO: Guided Practice (8 min)**

```
Docent: "Nu gaan WE samen één doen. Roep maar mee!"

[Toont nieuw voorbeeld]
Website bezoeken per uur op bol.com

Docent: "Oké, eerste vraag: Is TIJD belangrijk hier?"
[Wacht op antwoorden, studenten roepen "JA!"]

Docent: "Waarom?"
[Student aan het woord: "Want 's nachts minder bezoekers dan overdag"]

Docent: "Precies! En tweede vraag: Zijn intervallen regelmatig?"
[Student: "Ja, elk uur"]

Docent: "Dus wat is dit? Time series of sequential?"
[Groep roept: "TIME SERIES!"]

Docent doet nog 1 voorbeeld samen, nu met SEQUENTIAL:
Zoekgeschiedenis op Google van een gebruiker

[Zelfde proces, studenten participeren actiever]
```

#### **TRAFFIC LIGHT CHECK (1 min)**

```
Docent: "Even checken of iedereen het snapt."

Studenten tonen kleur kaartje (of hand op borst/hoofd/omhoog):
🟢 Groen: "Ik begrijp het en kan het uitleggen"
🟡 Oranje: "Ik begrijp het grotendeels maar heb vragen"
🔴 Rood: "Ik ben de draad kwijt"

Docent kijkt rond en telt:
- Veel groen: "Top, we gaan door!"
- Veel oranje/rood: "Ik zie veel oranje. Laat me nog 1 voorbeeld doen."
```

#### **YOU DO: Groepsopdracht (12 min)**

```
[Authentieke beroepspraktijk context]

Docent: "Jullie zijn data scientist bij een ziekenhuis.
De ICU vraagt: welke data kunnen we gebruiken voor early warning?"

Groepjes van 3-4, elke groep krijgt domein:
- Groep 1-2: ICU data (healthcare)
- Groep 3-4: Webshop data (e-commerce)
- Groep 5-6: Machine sensor data (industry)

OPDRACHT (10 min):
1. Brainstorm: Welke data verzamelt jullie organisatie?
2. Categoriseer:
   - 2 voorbeelden TIME SERIES
   - 2 voorbeelden SEQUENTIAL
3. Analyse (HBO niveau - EVALUEREN):
   - Waarom is dit onderscheid KRITIEK voor jullie organisatie?
   - Wat kan er fout gaan als je ze door elkaar haalt?

Voorbeeld:
"Als je hartslagdata (time series) behandelt als sequential,
verlies je temporele patronen → gemiste hartaanval waarschuwing!"

Docent loopt rond en:
- Stelt vragen: "Waarom denk je dat dit time series is?"
- Geeft hints: "Wat gebeurt er als je de tijd-volgorde verandert?"
- Checkt begrip: "Leg eens uit aan je groepsgenoot"

PLENUM DEEL (2 min):
Elke groep deelt 1 voorbeeld + waarom onderscheid belangrijk is
```

#### **Afsluiting Blok 1: Succescriteria check (1 min)**

```
Docent: "Terug naar onze succescriteria. Check voor jezelf:"

🎯 KUN JIJ NU:
□ Uitleggen wat time series data is?
□ Het verschil uitleggen?
□ Nieuwe voorbeelden categoriseren?
□ Uitleggen WAAROM dit belangrijk is?

"Steek hand op als je alle 4 kan checken."
[Docent ziet wie nog worstelt, maakt notitie voor extra support]
```

---

## MEETBARE DOELEN

Na implementatie verwachten we:

### Formatief handelen:
- **Was:** Exit ticket aan het einde (te laat)
- **Nu:** 6 formatieve checks tijdens de les
- **Meetbaar:** >70% studenten geeft aan "begrip" bij elke check

### Directe instructie:
- **Was:** Studenten beginnen zonder modeling
- **Nu:** Expliciete "I do, We do, You do" bij elk blok
- **Meetbaar:** Studenten scoren >80% op exit ticket vragen

### Modern HBO onderwijs:
- **Was:** Abstract voorbeeld, alleen toepassen
- **Nu:** Authentieke cases, evalueren en creëren
- **Meetbaar:** Studenten kunnen in exit ticket eigen beroepspraktijk voorbeeld geven

---

## EVALUATIE & BIJSTURING

### Na eerste keer geven:

**Vraag aan studenten (enquête):**
1. "De checks tijdens de les hielpen mij te weten of ik het snapte" (1-5)
2. "De voorbeelden waren relevant voor mijn toekomstig beroep" (1-5)
3. "Ik kon zelfstandig met de opdrachten aan de slag na de uitleg" (1-5)

**Observeer tijdens les:**
- Hoeveel studenten zitten vast tijdens hands-on? (moet <20% zijn)
- Hoeveel vragen tijdens "You do" zijn over "hoe" vs "waarom"?
  (meer "waarom" = goede modeling)

**Check leerdoelen:**
- Exit ticket resultaten: >80% correct moet haalbaar zijn
- Transfer vraag: >70% kan eigen beroepspraktijk voorbeeld geven

---

## CONCLUSIE

Deze les heeft **potentieel** maar mist cruciale elementen voor effectief HBO onderwijs:

**TOP 3 PRIORITEITEN:**
1. 🔴 Voeg formatieve checks toe TIJDENS de les
2. 🔴 Implementeer "I do, We do, You do" met modeling
3. 🟡 Gebruik authentieke beroepspraktijk case

**Tijdsinvestering:** 13 uur over 4 weken
**Verwachte impact:** Score 5.7/10 → 8.5/10

Met deze verbeteringen wordt dit een **voorbeeldige HBO les** die:
- ✅ Formatief stuurt op begrip
- ✅ Expliciet instrueert met modeling
- ✅ Verbindt met authentieke beroepspraktijk
- ✅ Stimuleert hogere-orde denken
- ✅ Zorgt voor transfer naar eigen context

---

**Volgende stappen:**
1. Bespreek dit plan met docententeam
2. Kies prioriteiten op basis van beschikbare tijd
3. Implementeer stapsgewijs (start met CRITICAL items)
4. Test met collega voordat je les geeft
5. Evalueer en bijsturen na eerste keer

**Succes! 🚀**
