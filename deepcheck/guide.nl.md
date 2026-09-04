---
title: "Gebruikershandleiding — DeepCheck"
---

DeepCheck is een app voor het diagnosticeren van de hardwarecomponenten van een smartphone: scherm, sensoren, camera, microfoon, luidsprekers, opslag, connectiviteitsmodules en meer. Alle tests worden **lokaal op het apparaat** uitgevoerd, zonder gegevens naar internet te verzenden.

Deze handleiding legt uit hoe je de app gebruikt en de tests uitvoert.

---

## Inhoud

1. [Algemene principes](#algemene-principes)
2. [Navigatie door de app](#navigatie-door-de-app)
3. [Sectie «Componenten»](#sectie-componenten)
4. [Lijst met tests](#lijst-met-tests)
5. [Modus «Serie»](#modus-serie)
6. [Stresstest van de processor](#stresstest-van-de-processor)
7. [RAM-test](#ram-test)
8. [Opslagtest](#opslagtest)
9. [GPU-test](#gpu-test)
10. [Sectie «Over het apparaat»](#sectie-over-het-apparaat)
11. [Instellingen](#instellingen)
12. [Pro-versie en beperkingen van de gratis modus](#pro-versie-en-beperkingen-van-de-gratis-modus)
13. [Machtigingen](#machtigingen)
14. [Veelgestelde vragen](#veelgestelde-vragen)

---

## Algemene principes

- De meeste tests zijn **interactief**: de app laat zien wat je moet doen (tikken, met je vinger vegen, je vinger erbij houden, naar geluid luisteren enz.) en jij bevestigt het resultaat: de test is **geslaagd** of **mislukt**.
- Na elke test wordt het resultaat vastgelegd: ✅ geslaagd of ❌ mislukt. Zo weet je welke componenten in orde zijn.
- Vóór tests die toegang tot hardware vereisen (camera, microfoon, sensoren, opslag) vraagt de app de bijbehorende **machtiging**. Zonder machtiging is de test beperkt.
- De app verzamelt je gegevens niet en verzendt ze nergens naartoe.

---

## Navigatie door de app

### Zijmenu (☰)

Wordt geopend met de knop met drie streepjes linksboven of door vanaf de linkerrand te vegen. Bevat de hoofdsecties:

- **Componenten** — lijst met 24 afzonderlijke tests van hardwarecomponenten.
- **Over het apparaat** — gedetailleerde informatie over de hardware en de specificaties van de smartphone.
- **Stresstest** — belastingstest van de processor.
- **RAM-test** — benchmark van het werkgeheugen.
- **Opslagtest** — benchmark van de opslagsnelheid.

### Menu met drie puntjes (⋮)

Wordt geopend met de knop rechtsboven. Bevat:

- **Instellingen** — keuze van thema, palet en taal.
- **Help** — opent deze handleiding.
- **Over de app** — versie, functies en informatie over de ontwikkelaar.

---

## Sectie «Componenten»

Dit is de hoofdsectie met de afzonderlijke tests. Kies de gewenste test uit de lijst en de app leidt je stap voor stap door de controle.

**Hoe een test verloopt:**

1. Open de test uit de lijst.
2. Lees de instructie op het startscherm (wat er en hoe het wordt gecontroleerd).
3. Start de controle en voer de gevraagde handelingen uit.
4. Bevestig het resultaat: werkt het component correct, markeer het dan als **geslaagd**; is er een probleem, markeer het dan als **mislukt**.

Na afloop keer je terug naar de lijst, waar te zien is welke tests al zijn uitgevoerd en met welk resultaat.

---

## Lijst met tests

De app bevat **24 tests**, gegroepeerd per componenttype.

### Scherm en aanraking

- **Schermtest** — controle van de kleurweergave en zoeken naar dode pixels (het scherm vullen met effen kleuren).
- **Aanraaktest** — controle van de respons van het hele aanraakoppervlak.
- **Multitouch-test** — controle van het gelijktijdig herkennen van meerdere aanrakingen.
- **Helderheidstest** — controle van de regeling van de helderheid van de achtergrondverlichting.

### Knoppen en biometrie

- **Knoppentest** — controle van de fysieke knoppen (volume, aan/uit enz.).
- **Vingerafdruktest** — controle van de vingerafdruksensor (er is minstens één toegevoegde vingerafdruk in de systeeminstellingen vereist).

### Geluid en trillen

- **Audiotest** — controle van de luidsprekers.
- **Koptelefoontest** — controle van een bedrade/draadloze headset.
- **Trillingstest** — controle van de trilmotor.

### Camera en flitser

- **Cameratest** — controle van de camera aan de voor- en achterkant.
- **Flitstest** — controle van de led-flitser.

### Voeding en opslag

- **Oplaadtest** — controle van de status en parameters van het opladen.
- **SD-kaarttest** — controle van het MicroSD-slot (er moet een kaart worden geplaatst).
- **OTG-test** — controle van de USB-OTG-ondersteuning (er moet een extern apparaat worden aangesloten).

### Connectiviteit

- **NFC-test** — controle van de NFC-module.
- **SIM-kaarttest** — controle van de detectie van SIM-kaarten.
- **Wi-Fi-test** — controle van de Wi-Fi-module.
- **Bluetooth-test** — controle van de Bluetooth-module.
- **GPS-test** — controle van de ontvangst van het satellietsignaal.

### Sensoren

- **Versnellingsmetertest** — controle van de versnellingssensor.
- **Gyroscooptest** — controle van de hoeksnelheidssensor.
- **Magnetometertest** — controle van het digitale kompas.
- **Lichttest** — controle van de omgevingslichtsensor.
- **Nabijheidstest** — controle van de nabijheidssensor (wordt bij het oor geactiveerd tijdens een gesprek).

> De set beschikbare tests hangt af van welke modules en sensoren jouw apparaat heeft.

---

## Modus «Serie»

Met de modus **«Serie»** kun je meerdere geselecteerde tests achter elkaar uitvoeren, zonder telkens naar de lijst terug te keren. Handig voor een snelle, uitgebreide controle van het apparaat (bijvoorbeeld voordat je een smartphone koopt of verkoopt).

- Selecteer de gewenste tests en start de serie.
- Tijdens de serie verschijnt onderaan een bedieningspaneel: naar de vorige/volgende test gaan, overslaan en beëindigen.
- Na afloop van de serie wordt een overzicht opgesteld: welke tests geslaagd, mislukt, overgeslagen of niet afgemaakt zijn.

> De modus «Serie» is beschikbaar in de **Pro**-versie.

---

## Stresstest van de processor

Belast alle cores van de processor en volgt in realtime het CPU-gebruik, de frequentie en de temperatuur van het apparaat. Wordt gebruikt om de stabiliteit en de koeling te controleren en throttling (frequentieverlaging door oververhitting) op te sporen.

**Parameters:**

- **Duur** — de looptijd van de test.
- **Belastingsniveau** — van zacht tot maximaal.
- **Belastingsprofiel:**
  - **Volledig** — integer-bewerkingen, SIMD/FP-rekenwerk, matrices en geheugen samen. Universele standaardmodus, dicht bij echte scenario's.
  - **FPU-torch** — maximale belasting van de floating-point-eenheid. De «heetste» modus; lokt het snelst throttling uit en onthult instabiliteit.
  - **Geheugen** — intensief werk met het geheugensubsysteem. Verwarmt de geheugencontroller en controleert de bandbreedte en stabiliteit van de RAM.

**Tijdens de test** worden grafieken van belasting en temperatuur getoond. Als een frequentieverlaging onder belasting wordt vastgesteld, meldt de app **throttling gedetecteerd**.

**Controlegeschiedenis** — de resultaten van de laatste runs worden bewaard, zodat je het gedrag van het apparaat op verschillende momenten of bij verschillende instellingen kunt vergelijken.

---

## RAM-test

Benchmark van het werkgeheugen. Meet de snelheid van schrijven, lezen, kopiëren en de toegangslatentie van het geheugen. De resultaten helpen de prestaties van het geheugensubsysteem van het apparaat te beoordelen.

> Op sommige apparaten kan de test in een **beperkte modus** werken, vanwege systeembeperkingen op de hoeveelheid toewijsbaar geheugen.

---

## Opslagtest

Benchmark van de opslagsnelheid: meet de werkelijke lees- en schrijfsnelheid.

- De **interne opslag** wordt gratis getest.
- **Externe opslag** (USB-OTG, SD-kaart) — de controle is beschikbaar in de **Pro**-versie.

**De USB-versie preciseren.** Bij het aansluiten van externe opslag kan de app aanbieden toegang tot het USB-apparaat toe te staan om een USB 3.0-station te onderscheiden van USB 2.0 bij aansluiting op een USB 2.0-poort van de telefoon. Dit is optioneel: de test start hoe dan ook, maar de nauwkeurigheid bij het bepalen van de kenmerken is dan lager.

> Houd er rekening mee: de werkelijke snelheid kan worden beperkt door de USB-poort van het apparaat zelf, niet door de opslag.

---

## GPU-test

Benchmark van de grafische processor om de kracht van apparaten te vergelijken met duidelijke maatstaven —**GFLOPS** en **FPS**— en om te controleren op throttling onder langdurige belasting.

Een run is **één continue fase** onder belasting:

- **GFLOPS** — rekenprestaties van de grafische kern, gemeten met een pure compute-berekening. Diezelfde belasting verwarmt de GPU, dus aan de hand van de daling van de GFLOPS in de tijd detecteert de app **throttling** (frequentieverlaging door oververhitting).
- **3D-scène (FPS)** — tijdens de GFLOPS-belasting meten korte tests de FPS van een 3D-scène (de belasting wordt even gepauzeerd zodat de meting nauwkeurig is). De FPS toont de terugval van de graphics bij oververhitting. De scène kan in de testinstellingen worden uitgeschakeld: dan blijft alleen de GFLOPS-meting over.

**Parameters:**

- **Duur** — van 2 tot 15 minuten. Runs korter dan 2 minuten worden niet in de geschiedenis bewaard: te weinig gegevens en throttling krijgt geen kans om zich te tonen.
- **3D-scène uitvoeren (FPS)** — de FPS-tests in-/uitschakelen.

De eerste ~30 seconden verlopen «koud»: zo wordt de piekprestatie vóór de opwarming vastgelegd. De test draait op volledig scherm met vergrendelde oriëntatie; het apparaat wordt merkbaar warm. Na afloop worden de piek en de gemiddelde GFLOPS, de FPS, de gedetecteerde throttling en de GPU-temperatuur getoond. De resultaten worden in de **runsgeschiedenis** bewaard.

> Hoe krachtiger de grafische kern, hoe hoger de GFLOPS en FPS. De resultaten zijn tussen apparaten vergelijkbaar, maar één synthetische test rangschikt verschillende architecturen (bijvoorbeeld Adreno en Mali) niet perfect; dat is normaal voor elke benchmark.
> Als het apparaat bij de start al warm was, kunnen de piek en de terugval te laag zijn: laat het afkoelen en start de test opnieuw.

---

## Sectie «Over het apparaat»

Een gedetailleerd overzicht van de hardware van de smartphone: processor, geheugen, scherm, camera's, sensoren, connectiviteitsmodules, Android-versie, beveiligingspatch en andere specificaties. Handig om te controleren of het overeenkomt met de opgegeven specificaties.

---

## Instellingen

Beschikbaar in het menu met drie puntjes → **Instellingen**:

- **Thema** — licht, donker of systeem.
- **Palet** — de kleuren van DeepCheck of van een van de verwante apps (Deedary, Seriary). Werkt samen met het thema: elk palet heeft zowel een lichte als een donkere variant.
- **Taal** — de taal van de interface (of de systeemtaal).

De instellingen worden meteen toegepast en blijven behouden tussen het opstarten van de app.

---

## Pro-versie en beperkingen van de gratis modus

De basistests zijn gratis beschikbaar. Een deel van de functies hoort bij de **Pro**-versie:

- **Modus «Serie»** — meerdere tests achter elkaar uitvoeren.
- **Resultaten exporteren naar PDF.**
- **Externe opslag testen** (USB-OTG en SD-kaarten). De interne opslag wordt gratis getest.
- **Onbeperkte runs** van de stresstest, de RAM-test, de opslagtest en de GPU-test (in de gratis modus is het aantal runs beperkt, met dezelfde limiet voor elk van deze tests).
- **Verlengde duur** van de stresstest.

In de gratis modus toont de app hoeveel runs er nog over zijn. Wanneer de limiet is bereikt, verschijnt een aanbod om over te stappen op Pro.

---

## Machtigingen

De app vraagt alleen machtigingen om specifieke hardware te controleren en **alleen op het moment** dat ze nodig zijn voor de bijbehorende test:

- **Camera** — voor de camera- en flitstest.
- **Microfoon** — voor de geluids-/opnamecontrole.
- **Locatie** — voor de GPS-test en het scannen van Wi-Fi.
- **Toegang tot bestanden/opslag** — voor de opslagtest.
- **Bluetooth, NFC enz.** — voor de bijbehorende connectiviteitstests.

Als je een machtiging hebt geweigerd, is de test beperkt. De machtiging kan later worden verleend in de systeeminstellingen van de app.

---

## Veelgestelde vragen

**De test start niet of de module wordt «niet gevonden».**
Waarschijnlijk heeft je apparaat de bijbehorende hardwaremodule niet (bijvoorbeeld NFC of een magnetometer), of is de vereiste machtiging niet verleend.

**De opslagsnelheid is lager dan verwacht.**
De werkelijke snelheid kan worden beperkt door de USB-poort van het apparaat, het type verbinding of de staat van de opslag.

**De stresstest toont throttling — is dat een defect?**
Niet per se. Frequentieverlaging onder langdurige belasting is een normaal beschermingsmechanisme tegen oververhitting. Sterke en vroege throttling kan wijzen op koelingsproblemen.

**Waar zijn mijn gegevens?**
Alle resultaten en metingen blijven op het apparaat. De app verzendt geen gegevens naar internet. Meer details in het Privacybeleid.

---

*Heb je nog vragen, schrijf dan naar de ontwikkelaar: **kotdikii@gmail.com***
