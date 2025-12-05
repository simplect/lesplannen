# Lesplan 2: Time Series Forecasting & Pattern Mining (2 uur)

## Leerdoelen
- LO8: Je kunt voorspellingen maken met ARMA/ARIMA
- LO9: Je kunt frequent voorkomende patronen herkennen (tijdreeksmotieven)

## Benodigdheden
- Jupyter notebook met ARIMA voorbeelden
- Datasets: verkoopcijfers, energieverbruik, sensor data
- Libraries: statsmodels, pmdarima, stumpy (voor motief-detectie)
- Flip-over of digibord voor gallery walk

---

## Opening (15 min)

**Activerende opdracht: "Voorspel de toekomst"**
- Toon grafiek: verkoopcijfers van 12 maanden
- Studenten individueel: teken vervolg voor komende 3 maanden
- Bespreek in tweetallen: op welke informatie baseer je je voorspelling?
- Plenum: "Jullie gebruiken patronen uit het verleden → dat doet ARIMA ook!"

---

## Blok 1: ARMA & ARIMA Intuïtie (35 min)

### Conceptuele opbouw (15 min)

**Stap 1: AR (AutoRegressive) - 5 min**
- Analogie: "Je humeur vandaag hangt af van gisteren en eergisteren"
- Formule: X_t = c + φ₁X_{t-1} + φ₂X_{t-2} + error
- Snelle poll: "Welke series heeft sterke AR? Temperatuur, dobbelsteen, aandelenkoers?"

**Stap 2: MA (Moving Average) - 5 min**
- "Je humeur hangt af van recente verrassingen/schokken"
- Formule: X_t = μ + θ₁ε_{t-1} + θ₂ε_{t-2} + ε_t
- Verschil AR vs MA uitleggen met visuals

**Stap 3: ARIMA - 5 min**
- I = Integrated = differencing voor stationariteit
- ARIMA(p,d,q): p=AR terms, d=differencing, q=MA terms
- Notatie uitleggen

### Hands-on experimenten (20 min)

Studenten in tweetallen met notebook:

```python
# Experiment 1: Speel met AR
# Maak synthetic data met verschillende φ waarden
# Wat gebeurt er bij φ > 1? Bij negatieve φ?

# Experiment 2: Fit ARIMA op echte data
# Stap 1: Check stationariteit (ADF test)
# Stap 2: Bepaal parameters met ACF/PACF plots
# Stap 3: Fit model
# Stap 4: Evalueer voorspellingen

# Reflectievraag: Waarom verschillen jullie modellen?
```

**Docent rol:**
- Loop rond voor support en stel verdiepende vragen
- "Waarom denk je dat deze parameter beter werkt?"
- "Wat betekent deze PACF plot voor je model?"

---

## **PAUZE (10 min)**

---

## Blok 2: Time Series Forecasting in praktijk (25 min)

### Case-based learning

Studenten werken in groepjes van 3:

**Scenario's (elk groepje krijgt één):**
1. **Retail:** Voorspel vraag naar zonnebrandcrème volgende zomer
2. **Energie:** Voorspel stroomverbruik komende week voor grid management
3. **Maintenance:** Voorspel wanneer machine onderhoud nodig heeft
4. **Finance:** Voorspel omzet volgende kwartaal

### Opdracht per groep (15 min):
- Analyseer gegeven historische data
- Bepaal ARIMA parameters
- Maak forecast
- Bereken confidence intervals
- Evalueer: Mean Absolute Error (MAE)

### Gallery walk (10 min):
- Groepen hangen resultaten op (visualisaties + key findings)
- Iedereen loopt rond en plaatst post-it met feedback/vragen
- Korte discussie: "Waarom verschillen forecasts tussen groepen?"

**Bespreekpunten:**
- Impact van parameterkeuzee
- Seizoensinvloeden herkennen
- Onzekerheid communiceren (confidence intervals)

---

## Blok 3: Tijdreeksmotieven (Pattern Mining) (30 min)

### Motivatie (5 min)
"Voorspellen is belangrijk, maar soms wil je terugkerende patronen herkennen"

**Voorbeelden tonen:**
- ECG: herkennen van hartslag patronen
- Website traffic: detecteren van gebruikersgedrag
- Manufacturing: kwaliteitsproblemen voorspellen

### Interactieve exploratie (20 min)

**Mini-lecture (5 min):**
- Wat zijn motieven? Subsequences die vaak voorkomen
- Toepassingen: anomaly detection, clustering, classification
- Technieken: Matrix Profile, Symbolic representation (SAX)

**Praktische oefening (15 min):**

Studenten individueel in notebook:

```python
# Dataset: sensor readings van productiemachine
# Opdracht 1: Vind top-3 meest voorkomende motieven
# Gebruik: stumpy library (Matrix Profile)
# Visualiseer gevonden motieven

# Opdracht 2: Link motieven aan events
# Welk motief correspondeert met:
# - Normale operatie
# - Start/stop fase
# - Mogelijke storing

# Reflectie: Hoe zou je dit gebruiken voor 
# predictive maintenance?
```

### Peer discussion (5 min):
- Vergelijk met buurpersoon: welke motieven vonden jullie?
- Zijn jullie het eens over interpretatie?
- Deel interessantste inzicht met de klas

---

## Afsluiting: Integratie & Reflectie (5 min)

### Groepsdiscussie:
"Wanneer gebruik je ARIMA vs. Motief-analyse?"
- ARIMA: forecasting, voorspellen van waarden
- Motieven: patroonherkenning, anomaly detection, clustering

### Final reflection (individueel):
Post in Teams/chat:
1. Wat is het verschil tussen voorspellen en patroonherkenning?
2. Noem één praktijktoepassing van vandaag die je interessant vindt
3. Wat wil je nog meer leren over time series?

**Afsluiting:**
- Bedank studenten voor participatie
- Verwijs naar aanvullende resources (online tutorials, papers)
- Preview volgende onderwerp in de cursus

---

## Algemene tips voor uitvoering

**Voorbereiding:**
- Zorg dat alle datasets werken en interessante patronen bevatten
- Test ARIMA fitting times (sommige modellen kunnen lang duren)
- Bereid extra uitdagingen voor snelle groepen
- Maak duidelijke rubric voor gallery walk beoordeling

**Tijdens de les:**
- Monitor groepswerk: zijn alle leden betrokken?
- Bij ARIMA: leg uit dat "trial and error" normaal is
- Wees flexibel met timing bij complexere analyses
- Stimuleer dat studenten fouten delen en ervan leren

**Differentiatie:**
- Minder ervaren: geef template code, focus op interpretatie
- Meer ervaren: laat parameter tuning optimaliseren, extra models (SARIMA, Prophet)
- Verschillende leerstijlen: visueel (plots), hands-on (code), conceptueel (discussie)

**Assessment mogelijkheden:**
- Observatie tijdens hands-on werk
- Kwaliteit van forecast + onderbouwing
- Bijdrage aan groepsdiscussies
- Exit tickets/reflecties analyseren

**Follow-up:**
- Deel goede voorbeelden van forecasts in Teams
- Optioneel: laat studenten eigen dataset analyseren als huiswerk
- Link naar volgende onderwerp: deep learning voor time series (LSTM)
