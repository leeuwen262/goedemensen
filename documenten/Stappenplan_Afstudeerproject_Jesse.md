# Uitgebreid Stappenplan Afstudeerproject - Signals Before Sales
## Jesse van Leeuwen | Goedemensen | Feb 2026 - Jun 2026

---

## 📋 OVERZICHT
**Totale duur:** 20 weken (100 dagen)  
**Hoofddoel:** Ontwikkelen van een beslissingsondersteunend sales-radar hulpmiddel  
**Deliverable:** Werkend Python/Jupyter prototype + eindrapport  

---

# FASE 1: ORIËNTATIE & SETUP (Week 1-2, ~10 dagen)

## Week 1: Eerste werkdag en kennismaking

### Dag 1-2: Onboarding & Toegang
- [ ] **Administratief regelen**
  - Werkplek en IT-middelen regelen
  - Toegang tot systemen aanvragen (Monday, Jobdigger, email, etc.)
  - Kennismaking met het team
  - Parkeren/reizen regelen indien nodig

- [ ] **Eerste gesprek met begeleiders**
  - Kickoff meeting met Peter Smit & Arthur Beemster
  - Verwachtingen afstemmen
  - Communicatiemomenten afspreken (bijv. wekelijkse check-ins)
  - Contact leggen met technische begeleider (Jerry/Tom/Anders/Andres Vlaeminck)

- [ ] **Werkplek inrichten**
  - Python development environment opzetten (Anaconda/Jupyter)
  - Git repository aanmaken voor je project
  - Folder structuur maken voor:
    - `/data` (raw, processed, external)
    - `/notebooks` (exploratie, analyse, modeling)
    - `/src` (herbruikbare code/functies)
    - `/docs` (documentatie, notities)
    - `/reports` (visualisaties, tussenrapportages)

### Dag 3-4: Systeemverkenning

- [ ] **Monday.com verkennen**
  - Inloggen en navigatie begrijpen
  - Meeting plannen met Peter/Arthur (1 uur) om door het systeem te lopen
  - Eventueel contact met Patrick (heeft velden uitgezocht)
  - Notities maken over:
    - Welke boards/tabellen er zijn
    - Welke velden relevant zijn voor jouw project
    - Hoe klantdata is georganiseerd
    - Hoe procesfases worden bijgehouden
    - Waar projecten en plaatsingen staan
    - Hoe communicatie/notities worden gelogd

- [ ] **Jobdigger verkennen**
  - Inloggen onder Arthur's account
  - Interface verkennen
  - Notities maken over:
    - Welke filters beschikbaar zijn
    - Welke data je kan exporteren
    - Welke analyses/rapporten er al zijn
    - Hoe vacaturedata eruitziet
    - Welke sectorinformatie beschikbaar is

- [ ] **API's onderzoeken**
  - Monday API documentatie bestuderen
  - Jobdigger export mogelijkheden checken (eerst exportfunctie proberen voordat je API demo aanvraagt)
  - Test exports maken van beide systemen

### Dag 5: Stakeholder interviews voorbereiden

- [ ] **Interview vragen voorbereiden voor accountmanagers**
  - Hoe bepalen ze nu welke klanten te benaderen?
  - Waar kijken ze naar online (websites, nieuwsbronnen)?
  - Wat maakt een klant "kansrijk" in hun ogen?
  - Welke signalen pikken ze nu op?
  - Wat zijn tijdrovende aspecten van acquisitie?
  - Hoe gebruiken ze Monday en Jobdigger nu?
  - Wat zou hen écht helpen?

- [ ] **Interviews plannen**
  - Minimaal 2 accountmanagers interviewen
  - Peter en Arthur interviewen over strategische visie
  - Sessies van 45-60 min inplannen

## Week 2: Data verzameling starten & context verdiepen

### Dag 6-7: Stakeholder interviews uitvoeren

- [ ] **Interviews houden**
  - Audio opnemen (met toestemming) of uitgebreide notities maken
  - Focus op:
    - Huidige werkwijze
    - Pijnpunten
    - Wensen voor het hulpmiddel
    - Welke info ze waardevol vinden
    - Hoe ze beslissingen nemen

- [ ] **Interview resultaten verwerken**
  - Transcripties maken (of samenvatten)
  - Belangrijkste inzichten clusteren
  - Pijnpunten en wensen prioriteren
  - Requirements lijst opstellen voor je tool

### Dag 8-10: Eerste data extractie

- [ ] **Monday data verzamelen**
  - Bepalen welke velden/boards relevant zijn
  - Eerste export maken (CSV of via API)
  - Data inladen in Python/Jupyter
  - Eerste inspectie:
    - Hoeveel records?
    - Welke kolommen?
    - Datakwaliteit?
    - Missing values?
    - Dataypes?

- [ ] **Jobdigger data verzamelen**
  - Export maken van relevante vacaturedata
  - Historische data verzamelen (minimaal 1-2 jaar terug)
  - Data inladen in Python
  - Eerste inspectie

- [ ] **Documentatie**
  - Data dictionary aanmaken (welke velden betekenen wat)
  - Data lineage documenteren (waar komt data vandaan)
  - Privacy/GDPR overwegingen noteren

### Tussentijdse deliverable (einde week 2):
✅ Werkende development environment  
✅ Toegang tot alle benodigde systemen  
✅ Interview inzichten gedocumenteerd  
✅ Eerste ruwe datasets verzameld  
✅ Weekly update voor begeleiders  

---

# FASE 2: DATA VERZAMELING & OPSCHONING (Week 3-5, ~20 dagen)

## Week 3: Exploratieve Data Analyse (EDA) - Monday data

### Dag 11-13: Monday CRM data verkennen

- [ ] **Klantgegevens analyseren**
  - Hoeveel unieke klanten?
  - Welke sectoren/branches?
  - Geografische spreiding?
  - Actieve vs inactieve klanten

- [ ] **Projecthistorie analyseren**
  - Hoeveel projecten per klant?
  - Tijdsduur van projecten
  - Succes/plaatsingsratio
  - Gemiddelde tijd tussen projecten
  - Seasonal patterns?

- [ ] **Communicatiedata analyseren**
  - Contactmomenten per klant
  - Type communicatie (email, telefoon, meeting)
  - Frequentie van contact
  - Laatste contactmoment per klant

- [ ] **Procesfase data analyseren**
  - Welke fases worden doorlopen?
  - Conversion rates tussen fases
  - Gemiddelde doorlooptijd per fase
  - Drop-off points

### Dag 14-15: Visualisaties en patronen

- [ ] **Visualisaties maken**
  - Tijdlijn van projecten per klant
  - Heatmaps van activiteit
  - Funnel visualisaties
  - Client engagement scores

- [ ] **Patronen identificeren**
  - Welke klanten zijn meest actief?
  - Wat onderscheidt succesvolle trajecten?
  - Zijn er seizoenspatronen?
  - Hoe lang duurt het van eerste contact tot plaatsing?

## Week 4: Exploratieve Data Analyse (EDA) - Jobdigger data

### Dag 16-18: Jobdigger arbeidsmarktdata verkennen

- [ ] **Vacaturedata analyseren**
  - Aantal vacatures per sector/branche
  - Trending profielen
  - Geografische concentraties
  - Prijsniveaus
  - Tijdspatronen (wanneer worden vacatures gepost?)

- [ ] **Sector analyses**
  - Welke sectoren zijn het actiefst?
  - Groeicijfers per sector
  - Vergelijking publiek vs privaat

- [ ] **Koppeling met Monday-klanten**
  - Kunnen we klanten matchen met sectoren in Jobdigger?
  - Bij welke klanten zien we veel vacature-activiteit?
  - Bij welke klanten zien we juist weinig?

### Dag 19-20: Data kwaliteit en opschoning

- [ ] **Data cleaning Monday**
  - Missing values aanpakken
  - Duplicaten verwijderen
  - Inconsistenties oplossen
  - Datums standardiseren
  - Tekstvelden normaliseren

- [ ] **Data cleaning Jobdigger**
  - Relevante vacatures filteren
  - Bedrijfsnamen normaliseren (voor matching)
  - Sectorcategorieën harmoniseren

- [ ] **Documentatie opschoning**
  - Alle transformaties documenteren
  - Scripts maken voor reproduceerbare cleaning
  - Data quality report maken

## Week 5: Data integratie en feature engineering

### Dag 21-23: Data koppeling

- [ ] **Matching strategie ontwikkelen**
  - Hoe koppelen we Jobdigger vacatures aan Monday klanten?
  - Bedrijfsnaam matching (fuzzy matching nodig?)
  - Sector/branche matching
  - Eventueel handmatige mapping table maken

- [ ] **Integratie uitvoeren**
  - Datasets samenvoegen
  - Relaties leggen tussen entiteiten
  - Master dataset creëren

### Dag 24-25: Feature engineering

- [ ] **CRM-gebaseerde features maken**
  - `days_since_last_contact`: Hoe lang geleden laatste contact?
  - `total_projects`: Totaal aantal projecten met klant
  - `avg_project_duration`: Gemiddelde projectduur
  - `contact_frequency`: Hoe vaak per maand contact?
  - `conversion_rate`: Historische succesratio
  - `days_since_last_project`: Recency van laatste project
  - `active_projects`: Huidige lopende projecten
  - `project_gap_avg`: Gemiddelde tijd tussen projecten
  - `total_revenue`: Totale omzet van klant (indien beschikbaar)

- [ ] **Arbeidsmarkt-gebaseerde features maken**
  - `recent_vacancies_count`: Aantal vacatures laatste 30/60/90 dagen
  - `vacancy_growth_rate`: Groei in vacatures t.o.v. vorige periode
  - `sector_activity_score`: Hoe actief is de sector momenteel?
  - `profile_match_score`: Match tussen onze expertise en hun vacatures
  - `avg_vacancy_price`: Prijsniveau van vacatures
  - `new_vacancies_this_week`: Hele recente vacatures

- [ ] **Combinatie features**
  - `opportunity_score_v1`: Eerste poging om kans te kwantificeren
  - `engagement_momentum`: Is er recent momentum in de relatie?
  - Experimenteer met verschillende combinaties

### Dag 25: Check-in en reflectie

- [ ] **Mid-project review**
  - Stand van zaken bespreken met begeleiders
  - Data quality review
  - Features bespreken
  - Bijsturen waar nodig

### Tussentijdse deliverable (einde week 5):
✅ Schone, geïntegreerde dataset  
✅ Feature engineering gedocumenteerd  
✅ EDA rapport met visualisaties  
✅ Data dictionary compleet  
✅ Weekly update voor begeleiders  

---

# FASE 3: ANALYSE & MODELLERING (Week 6-10, ~25 dagen)

## Week 6: Model strategie bepalen

### Dag 26-27: Literatuuronderzoek & model opties

- [ ] **Literatuur bestuderen**
  - Decision Support Systems (Power, 2002)
  - Explainable AI (Molnar, 2022)
  - Lead scoring modellen
  - Recommender systems

- [ ] **Model opties evalueren**
  - **Optie 1: Rule-based scoring**
    - Pro's: Zeer uitlegbaar, eenvoudig te implementeren
    - Con's: Minder flexibel, handmatig tunen
  
  - **Optie 2: Similarity-based (collaborative filtering)**
    - Pro's: Uitlegbaar ("klant X lijkt op klant Y die recent..."), geen labels nodig
    - Con's: Cold start probleem voor nieuwe signalen
  
  - **Optie 3: Supervised learning (als labels beschikbaar)**
    - Pro's: Kan patronen leren, voorspellend
    - Con's: Vereist goede labels, minder uitlegbaar
  
  - **Optie 4: Hybrid approach**
    - Combinatie van bovenstaande

### Dag 28-30: Baseline model ontwikkelen

- [ ] **Eenvoudig scoring model bouwen**
  - Weighted scoring op basis van:
    - Recency (laatste contact)
    - Frequency (aantal projecten)
    - Monetary (omzet/waarde)
    - Market activity (Jobdigger signalen)
  
- [ ] **Scoring formule opstellen**
  ```
  Priority_Score = 
    w1 * recency_score +
    w2 * frequency_score +
    w3 * monetary_score +
    w4 * market_activity_score
  ```

- [ ] **Weights bepalen**
  - Eerste poging: gelijk verdelen
  - Tweede poging: op basis van stakeholder input
  - Derde poging: op basis van historische validatie

- [ ] **Baseline evalueren**
  - Top 10 klanten genereren
  - Met accountmanagers bespreken: herkennen ze dit?
  - Feedback verzamelen
  - Itereren

## Week 7-8: Geavanceerder model ontwikkelen

### Dag 31-35: Labels onderzoeken (indien beschikbaar)

- [ ] **Label definitie bepalen**
  - Wat is "succes"? → Plaatsing binnen X weken na contact?
  - Historische data: welke contactmomenten leidden tot plaatsingen?
  - Kunnen we dit uit Monday data halen?

- [ ] **Als labels beschikbaar zijn: Supervised learning**
  - [ ] Dataset splitsen (train/test, let op temporal split!)
  - [ ] Features selecteren
  - [ ] Model opties proberen:
    - Logistic Regression (start eenvoudig!)
    - Random Forest
    - XGBoost
  - [ ] Focus op interpretability:
    - Feature importance
    - SHAP values voor uitleg
    - Partial dependence plots

- [ ] **Als labels NIET goed beschikbaar zijn: Alternative approaches**
  - [ ] Unsupervised clustering
    - Groepeer klanten in segmenten
    - Analyseer karakteristieken per segment
    - Identificeer "hoog potentieel" clusters
  
  - [ ] Anomaly detection
    - Detecteer afwijkingen in klantgedrag
    - Detecteer afwijkende marktactiviteit
    - Combineer beide voor opportunity detection
  
  - [ ] Time series analysis
    - Voorspel vacature trends per sector
    - Voorspel klant engagement cycli
    - Identificeer optimale contact momenten

### Dag 36-40: Model verfijnen en tunen

- [ ] **Hyperparameter tuning**
  - Grid search of random search
  - Cross-validation (let op: time-series aware!)

- [ ] **Feature engineering iteratie 2**
  - Op basis van feature importance nieuwe features bedenken
  - Interactie features toevoegen
  - Polynomiale features proberen

- [ ] **Model ensemble overwegen**
  - Combineer meerdere modellen
  - Voting of stacking

## Week 9: Explainability & interpretatie

### Dag 41-43: Uitlegbaarheid bouwen

- [ ] **SHAP values implementeren**
  - Voor elk voorspelling: waarom deze score?
  - Visualisaties maken (waterfall plots, force plots)

- [ ] **Feature contribution berekenen**
  - Per klant: welke factoren dragen het meest bij?
  - Categoriseer bijdragen:
    - 🟢 Positieve signalen (verhogen kans)
    - 🔴 Negatieve signalen (verlagen kans)

- [ ] **Natuurlijke taal explanations**
  - Template-based explanations genereren:
    - "Klant X is kansrijk omdat:"
    - "- Laatste project was Y maanden geleden (normale cyclus is Z)"
    - "- In hun sector zijn vacatures met 30% gestegen"
    - "- Ze hebben recent 3 nieuwe vacatures gepost"

### Dag 44-45: Backtesting en validatie

- [ ] **Historische validatie**
  - Simuleer: wat zou model hebben voorspeld 3/6/12 maanden geleden?
  - Vergelijk met wat er daadwerkelijk gebeurde
  - Niet als harde metric, maar als sanity check

- [ ] **Edge cases testen**
  - Wat doet model met nieuwe klanten? (cold start)
  - Wat met inactieve klanten?
  - Wat met klanten met veel projecten maar weinig recent?

## Week 10: Prototype bouwen

### Dag 46-50: Interactief prototype

- [ ] **Jupyter dashboard/interface maken**
  - Input: selecteer datum
  - Output: prioriteitslijst klanten
  - Voor elke klant:
    - Priority score (1-10 of High/Medium/Low)
    - Explanation (waarom deze score)
    - Aanbevolen acties
    - Relevante data points

- [ ] **Visualisaties toevoegen**
  - Top 20 klanten ranked list
  - Sector heatmap (welke sectoren zijn hot)
  - Timeline: wanneer was laatste contact
  - Vacancy trends per klant

- [ ] **Export functionaliteit**
  - Genereer Excel/CSV met prioriteitenlijst
  - Mogelijkheid om te filteren (sector, regio, etc.)

- [ ] **(Optioneel) Monday integratie voorbereiden**
  - Script om status te updaten via API
  - Proof of concept: kan het?
  - Volledige implementatie is buiten scope, maar laat zien dat het kan

### Tussentijdse deliverable (einde week 10):
✅ Werkend model met uitlegbaarheid  
✅ Jupyter notebook prototype  
✅ Model documentatie  
✅ Backtesting resultaten  
✅ Demo klaar voor evaluatie  

---

# FASE 4: EVALUATIE (Week 11-13, ~15 dagen)

## Week 11: Kwalitatieve evaluatie voorbereiden

### Dag 51-53: Evaluatie sessies plannen

- [ ] **Evaluatie protocol opstellen**
  - Welke scenario's testen we?
  - Welke vragen stellen we?
  - Hoe meten we "herkenbaarheid" en "uitlegbaarheid"?

- [ ] **Test cases voorbereiden**
  - 10-15 klanten selecteren (mix van verschillende profielen)
  - Voor elk: model output genereren
  - Vergelijk met accountmanager's eigen prioritering

- [ ] **Evaluatie sessies inplannen**
  - 4-5 sessies met verschillende accountmanagers
  - 1-1.5 uur per sessie
  - Peter en Arthur ook evalueren laten doen

### Dag 54-55: Evaluatie criteria uitwerken

- [ ] **Uitlegbaarheid meten**
  - Schaal 1-5: Begrijp je waarom deze klant deze score heeft?
  - Open vraag: Wat maakt het (on)duidelijk?

- [ ] **Herkenbaarheid meten**
  - Schaal 1-5: Herken je deze prioritering?
  - Welke klanten zou je anders prioriteren en waarom?

- [ ] **Bruikbaarheid meten**
  - Schaal 1-5: Zou dit je helpen in je dagelijkse werk?
  - Wat ontbreekt er?
  - Wat zou anders moeten?

## Week 12-13: Evaluatie uitvoeren en verwerken

### Dag 56-62: Evaluatie sessies

- [ ] **Sessies uitvoeren**
  - Prototype demonstreren
  - Feedback verzamelen (notities + opname)
  - Laat accountmanagers het zelf gebruiken

- [ ] **A/B scenario's testen**
  - Laat ze eerst zelf top 10 maken (zonder tool)
  - Toon daarna tool output
  - Bespreek verschillen en overeenkomsten

- [ ] **Verbeterpunten identificeren**
  - Wat werkt goed?
  - Wat niet?
  - Quick wins die je nog kan implementeren?

### Dag 63-65: Feedback verwerken en itereren

- [ ] **Evaluatie resultaten analyseren**
  - Kwantitatieve scores samenvatten
  - Kwalitatieve feedback clusteren
  - Patroon herkennen in feedback

- [ ] **Quick wins implementeren**
  - Als bepaalde feedback snel op te lossen is, doe het
  - Kleine UI verbeteringen
  - Extra uitleg toevoegen

- [ ] **Finale model versie**
  - Laatste aanpassingen doorvoeren
  - Versie 1.0 "bevriezen"
  - Documenteren wat in v2.0 zou kunnen

### Tussentijdse deliverable (einde week 13):
✅ Evaluatie resultaten gedocumenteerd  
✅ Gebruikersfeedback samengevat  
✅ Verbeteringen doorgevoerd  
✅ Finale prototype versie  

---

# FASE 5: RAPPORTAGE & AFSLUITING (Week 14-20, ~10 dagen productief werk)

## Week 14-16: Eindrapport schrijven

### Dag 66-70: Hoofdstukken schrijven

- [ ] **Inleiding (2-3 pagina's)**
  - Context schetsen
  - Probleemstelling
  - Doel en relevantie
  - Leeswijzer

- [ ] **Theoretisch kader (5-7 pagina's)**
  - Decision Support Systems
  - Lead scoring / opportunity detection
  - Explainable AI
  - Relevante modellen en technieken

- [ ] **Methoden (8-10 pagina's)**
  - Onderzoeksopzet
  - Data bronnen (Monday, Jobdigger)
  - Data verzameling en opschoning
  - Feature engineering
  - Model ontwikkeling
  - Evaluatie aanpak

- [ ] **Resultaten (10-12 pagina's)**
  - EDA bevindingen
  - Model prestaties
  - Uitlegbaarheid voorbeelden
  - Evaluatie resultaten
  - Gebruikersfeedback

- [ ] **Discussie (5-7 pagina's)**
  - Interpretatie van resultaten
  - Beantwoording onderzoeksvragen
  - Sterke punten van de aanpak
  - Beperkingen en kanttekeningen
  - Vergelijking met literatuur

- [ ] **Conclusie & Aanbevelingen (3-5 pagina's)**
  - Beantwoording hoofdvraag
  - Praktische aanbevelingen voor Goedemensen
  - Toekomstig onderzoek
  - Implementatie roadmap

### Dag 71-75: Rapport afwerken

- [ ] **Visualisaties en tabellen**
  - Alle figuren high-quality exporteren
  - Tabellen netjes formatteren
  - Captions en numbering controleren

- [ ] **Appendices**
  - Interview vragen
  - Data dictionary
  - Feature beschrijvingen
  - Code snippets (de belangrijkste)
  - Evaluatie vragenlijst

- [ ] **Bibliografie**
  - Alle bronnen in APA stijl
  - Controleer op volledigheid

- [ ] **Abstract/Samenvatting**
  - Nederlandse samenvatting (1 pagina)
  - Engelse abstract (1 pagina)

### Dag 76-78: Review en polish

- [ ] **Zelf doorlezen**
  - Rode draad controleren
  - Spelling en grammatica
  - Consistentie in terminologie
  - Figuur/tabel referenties kloppen

- [ ] **Feedback vragen**
  - Peter en Arthur laten lezen (management summary)
  - Technische begeleider laten reviewen (methoden/resultaten)
  - Medestudent voor peer review

- [ ] **Revisies doorvoeren**
  - Feedback verwerken
  - Laatste puntjes op de i

## Week 17-18: Presentatie en implementatie advies

### Dag 79-82: Eindpresentatie voorbereiden

- [ ] **PowerPoint maken (15-20 slides)**
  - Introductie (1-2 slides)
  - Probleem en doel (2 slides)
  - Aanpak (3-4 slides)
  - Demo/resultaten (5-6 slides)
  - Evaluatie (2-3 slides)
  - Conclusies en aanbevelingen (2-3 slides)
  - Q&A

- [ ] **Demo voorbereiden**
  - Live demo scenario
  - Backup screenshots/video voor als iets niet werkt
  - Test je demo vooraf!

- [ ] **Presentatie oefenen**
  - Timing checken (meestal 20-30 min presentatie)
  - Voor collega's of vrienden presenteren
  - Feedback vragen en aanpassen

### Dag 83-85: Implementatie advies

- [ ] **Technische documentatie**
  - README voor je code
  - Installatie instructies
  - Hoe data te updaten
  - Hoe model te runnen
  - Troubleshooting guide

- [ ] **Implementatie roadmap maken**
  - **Fase 1 (korte termijn)**: Handmatig gebruik prototype
  - **Fase 2 (middellange termijn)**: Automatisering + Monday integratie
  - **Fase 3 (lange termijn)**: Uitbreidingen en nieuwe features
  - Voor elke fase: wat is nodig, geschatte tijd, kosten, risico's

- [ ] **Overdracht voorbereiden**
  - Wie neemt het over?
  - Welke kennis moet overgedragen?
  - Documentatie compleet maken

## Week 19: Buffer en eindcontrole

### Dag 86-90: Final checks en buffer

- [ ] **Code review en cleanup**
  - Overbodige code verwijderen
  - Commentaar toevoegen waar nodig
  - Notebooks netjes maken (markdown cells)
  - Reproduceerbaar maken

- [ ] **Repository organiseren**
  - README.md met project overview
  - requirements.txt met alle dependencies
  - Folder structuur logisch
  - Data (anonymized sample) toevoegen voor reproduceerbaarheid

- [ ] **Laatste tests**
  - Kan iemand anders je code draaien?
  - Werkt alles nog na cleanup?
  - Zijn alle bestanden er?

- [ ] **Eindversies exporteren**
  - Rapport als PDF
  - Presentatie als PDF (en .pptx backup)
  - Code op USB stick of GitLab/GitHub
  - Alles wat school nodig heeft

## Week 20: Afsluiten en inleveren

### Dag 91-95: Eindspurt

- [ ] **Formele inlevering voorbereiden**
  - Check inlever requirements van school
  - Alle benodigde formulieren invullen
  - Beoordelingsformulier klaarzetten voor begeleiders

- [ ] **Finale presentatie geven**
  - Bij Goedemensen
  - Voor school (indien vereist)

- [ ] **Inleveren!**
  - Deadline: Maandag 8 juni 2026 vóór 13:00 uur
  - Op tijd inleveren (doe niet last-minute!)

- [ ] **Examen voorbereiden**
  - Examenzittingen: 22 juni - 8 juli 2026
  - Mogelijke verdedigingsvragen voorbereiden
  - Je werk nog eens goed doorlezen

### Dag 96-100: Afronding en overdracht

- [ ] **Afsluitende meeting Goedemensen**
  - Finale presentatie en demo
  - Overdracht documentatie
  - Feedbackgesprek
  - Bedanken voor de samenwerking!

- [ ] **Reflectie**
  - Wat heb je geleerd?
  - Wat ging goed?
  - Wat zou je anders doen?
  - Portfolio item maken van dit project

---

# 📅 WEEKSCHEMA OVERZICHT

| Week | Fase | Focus | Deliverables |
|------|------|-------|-------------|
| 1-2 | Oriëntatie | Setup, interviews, eerste data | Werkende omgeving, interview inzichten |
| 3-5 | Data | EDA, cleaning, integratie, features | Schone dataset, features, EDA rapport |
| 6-10 | Modellering | Model ontwikkeling, verfijning, prototype | Werkend model + prototype |
| 11-13 | Evaluatie | Gebruikerstesten, feedback, iteratie | Evaluatie resultaten, finale versie |
| 14-18 | Rapportage | Eindrapport, presentatie, implementatie advies | Eindrapport, presentatie, documentatie |
| 19-20 | Afsluiting | Buffer, eindcontrole, inlevering | Ingeleverd werk, examen gereed |

---

# 🎯 BELANGRIJKE MIJLPALEN

- **Week 2**: Eerste data in handen, begrip van systemen ✅
- **Week 5**: Schone, geïntegreerde dataset klaar ✅
- **Week 10**: Werkend prototype gereed voor evaluatie ✅
- **Week 13**: Evaluatie afgerond, finale versie ✅
- **Week 18**: Eindrapport concept klaar ✅
- **8 Juni 2026**: INLEVEREN! 🎓

---

# 💡 TIPS & BEST PRACTICES

## Wekelijkse routine
- [ ] **Maandag**: Weekplanning maken, prioriteiten stellen
- [ ] **Woensdag**: Midweek check-in met jezelf (on track?)
- [ ] **Vrijdag**: Weekly update naar begeleiders (email/kort gesprek)
  - Wat heb je deze week gedaan?
  - Wat ga je volgende week doen?
  - Waar loop je tegenaan?
  - Hulp nodig?

## Documentatie
- 📝 **Notities dagelijks bijhouden**: Wat deed je, waarom, wat was het resultaat?
- 📊 **Versie beheer**: Git commits met duidelijke messages
- 📸 **Screenshots**: Van interessante analyses, voor in je rapport
- 💭 **Reflectie logboek**: Lessen, inzichten, ideeën voor later

## Code best practices
- ✅ Functioneel programmeren (herbruikbare functies)
- ✅ Duidelijke variabele namen
- ✅ Commentaar bij complexe code
- ✅ Notebooks met markdown uitleg (alsof je het voorstelt)
- ✅ Requirements.txt vanaf het begin bijhouden

## Communicatie
- 🗓️ **Vaste overlegmomenten** met begeleiders inplannen
- 💬 **Proactief communiceren** bij problemen (niet wachten!)
- 🤝 **Stakeholders betrokken houden** (ze zijn je "klanten")
- ❓ **Geen domme vragen** - liever te veel vragen dan te weinig

## Timemanagement
- ⏰ **Time-boxing**: Geef taken een max tijd, voorkom rabbit holes
- 🎯 **80/20 regel**: Perfect is de vijand van goed
- 📅 **Buffer inbouwen**: Planning is altijd te optimistisch
- 🚫 **Scope creep voorkomen**: Blijf bij je afgebakende scope!

## Gezondheid en energie
- 🏃 **Regelmatig pauzeren**: Pomodoro techniek (25 min werk, 5 min pauze)
- 🥗 **Goed eten en slapen**: Je brein heeft brandstof nodig
- 🌳 **Af en toe losweken**: Voorkom burn-out
- 🎉 **Mijlpalen vieren**: Motivatie houden!

---

# 🚨 RISICO'S & MITIGATIE

| Risico | Kans | Impact | Mitigatie |
|--------|------|--------|-----------|
| Data kwaliteit slecht | Midden | Hoog | Early EDA, tijd voor cleaning inplannen |
| Geen goede labels beschikbaar | Hoog | Midden | Plan B: unsupervised/similarity approaches |
| API toegang problemen | Laag | Midden | Start met exports, API als nice-to-have |
| Model niet uitlegbaar genoeg | Midden | Hoog | Vanaf begin focus op explainability |
| Scope creep | Hoog | Hoog | Strict houden aan plan, "nice to have" lijst |
| Technische issues | Midden | Midden | Backup maken, early tests, vraag hulp |
| Evaluatie negatief | Laag | Hoog | Tussentijdse feedback loops, iteratief werken |
| Timing issues | Midden | Hoog | Buffer weken 19-20, wekelijks monitoren |

---

# 📚 RESOURCES & LINKS

## Literatuur (te bestuderen)
- Power, D. J. (2002). Decision support systems: Concepts and resources for managers
- Molnar, C. (2022). Interpretable machine learning
- Hevner et al. (2004). Design science in information systems research
- Amershi et al. (2019). Guidelines for human-AI interaction

## Tools & Libraries
- **Data:** pandas, numpy
- **Visualisatie:** matplotlib, seaborn, plotly
- **Modeling:** scikit-learn, xgboost (indien supervised)
- **Explainability:** shap, lime
- **APIs:** requests, monday Python SDK
- **Notebooks:** Jupyter Lab

## Nuttige links
- Monday API docs: https://developer.monday.com/
- Jobdigger: (interne toegang via Arthur)
- SHAP documentation: https://shap.readthedocs.io/

---

# ✅ CHECKLIST EERSTE WEEK

Voor jouw **eerste werkdag morgen**, focus op:

### Dag 1 (Morgen!) - Prioriteiten:
1. ✅ Werkplek regelen en systemen toegang
2. ✅ Kickoff meeting met Peter & Arthur plannen
3. ✅ Python environment opzetten op je laptop
4. ✅ Project folder structuur maken
5. ✅ Eerste verkenning Monday (rondkijken, geen diepte analyse)
6. ✅ Contact opnemen met technische begeleider (Jerry/Tom/Anders)

### Gesprekspunten voor kickoff:
- Wekelijkse check-ins afspreken (wanneer, hoe lang)
- Verwachtingen wederzijds bespreken
- Toegang tot Monday & Jobdigger regelen
- Wanneer kan ik accountmanagers interviewen?
- Data privacy/GDPR richtlijnen bespreken

---

**Succes met je eerste werkdag en je afstudeerproject, Jesse! 🚀**

*Laatste update: 9 februari 2026*
