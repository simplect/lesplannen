# Lesplan 1: Time Series Data & Preprocessing (2 uur)

## Leerdoelen
- LO6: Je kunt uitleggen wat time series data is en hoe het verschilt van sequentiële data
- LO7: Je kunt technieken uitleggen voor het transformeren van tijdreeksdata

## Benodigdheden
- Jupyter notebook met voorbeelden (temperatuurdata, aandelenkoersen, IoT-sensoren)
- Dataset: uurlijkse energieverbruik data of vergelijkbaar
- Pandas, matplotlib, statsmodels libraries

---

## Les 1: Structuur

### Opening (15 min)

**Activatie: "Wat zie je?"**
- Toon 3 visualisaties zonder labels:
  1. Dagelijkse temperatuur over een jaar
  2. Tekst als sequence (lettervolgorde)
  3. Sensor readings over tijd
  
- Studenten in tweetallen: "Welke twee lijken op elkaar? Waarom?"
- Plenum: Verzamel antwoorden → leid in: *tijd als cruciale dimensie*

### Blok 1: Time Series vs Sequential Data (25 min)

**Mini-lecture (10 min)**
- Definitie time series: observaties geordend in tijd met *regelmatige intervallen*
- Verschil met sequentiële data: tijd is intrinsiek belangrijk vs. volgorde belangrijk
- Voorbeelden laten categoriseren door studenten:
  - DNA-sequentie → sequential
  - Hartslag per seconde → time series
  - Zoekgeschiedenis → sequential
  - Dagelijkse verkoopcijfers → time series

**Groepsopdracht (15 min)**
Studenten in groepjes van 3-4:
- Elke groep krijgt een domein (zorg, retail, industrie, transport)
- Bedenk 2 time series voorbeelden en 2 sequential data voorbeelden uit dat domein
- Waarom is het onderscheid belangrijk voor analyse?
- Plenum: elk groepje deelt 1 voorbeeld

---

### Blok 2: Karakteristieken van Time Series (30 min)

**Interactieve verkenning (20 min)**
Studenten werken in notebook:

```python
# Gegeven: energieverbruik dataset
# Opdracht 1: Visualiseer de data
# Opdracht 2: Identificeer componenten:
# - Trend (stijgend/dalend patroon)
# - Seizoensinvloed (herhalend patroon)
# - Ruis (onregelmatige fluctuaties)
```

**Think-Pair-Share:**
- Individual: Welke component zie je het sterkst?
- Pair: Vergelijk met buurpersoon
- Share: 3 studenten delen bevindingen

**Mini-lecture (10 min)**
- Formeel introduceren: Trend, Seasonality, Noise
- Stationariteit concept: "waarom is dit belangrijk?"
- Visual: stationaire vs. non-stationaire series

---

### **PAUZE (10 min)**

---

### Blok 3: Data Transformatie Technieken (35 min)

**Probleemstelling (5 min)**
Toon "vuile" tijdreeks met:
- Missing values
- Outliers
- Veel ruis
- Verschillende schalen

"Hoe maken we dit analyseerbaar?"

**Hands-on workshop (25 min)**

Studenten werken individueel door notebook met 4 technieken:

**1. Dealing with missing data (6 min)**
```python
# Forward fill, backward fill, interpolatie
# Wanneer gebruik je welke?
```

**2. Noise reduction (7 min)**
```python
# Moving average
# Exponential smoothing
# Experimenteer met window sizes
```

**3. Normalisatie (6 min)**
```python
# Min-max scaling
# Z-score normalization
# Waarom is dit nodig voor vergelijking?
```

**4. Outlier detection (6 min)**
```python
# Statistical methods (z-score, IQR)
# Visualisatie boxplot
```

**Peer review (5 min)**
- Wissel notebooks met buurpersoon
- Bekijk elkaars transformaties
- "Welke aanpak werkt het beste voor deze data?"

---

### Afsluiting (5 min)

**Exit ticket (individueel, in notebook of op papier):**
1. Noem één verschil tussen time series en sequential data
2. Welke transformatietechniek zou je gebruiken voor sensor data met veel ruis?
3. Één vraag die je nog hebt

**Preview volgende les:** "Nu we data kunnen voorbereiden, gaan we voorspellingen maken met ARIMA!"

---

## Algemene tips voor uitvoering

**Differentiatie:** 
- Voorzie snelle studenten van extra challenge opdrachten in notebooks
- Zorg dat notebooks stap-voor-stap opgebouwd zijn met hints

**Formative assessment:** 
- Loop rond, stel vragen, observeer discussies
- Check begrip tijdens hands-on momenten

**Time management:** 
- Gebruik timer, wees strikt met pauzes
- Houd 5 minuten buffer voor onverwachte vragen

**Technische setup:** 
- Test alle code vooraf, heb backup plan bij tech issues
- Zorg dat datasets vooraf geladen zijn in notebooks

**Aanpassingsmogelijkheden:**
- Bij minder programmeerervaring: meer begeleide code, minder zelfstandig
- Bij meer ervaring: minder structuur, meer open opdrachten
- Hybrid/online: gebruik breakout rooms, collaborative notebooks, Mentimeter voor polls
