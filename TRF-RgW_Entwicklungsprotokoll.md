# TRF-RgW – Entwicklungsprotokoll  
## Thermochemischer Reaktor mit Festoxid-Reduktion und gekoppelter Wärmerückführung  
**Autor:** Frank Robert Poppe  
**Projektstatus:** Offen, in Entwicklung  
**Lizenz:** CC BY-NC-SA 4.0  
**Letzte Aktualisierung:** 2025-04-20

---

## 🔍 Ziel des Projekts

Das TRF-RgW-System soll einen modularen, vollständig autarken Festkörperreaktor ermöglichen, der durch rein thermochemische Prozesse elektrische Energie erzeugt – **ohne bewegliche Teile, ohne externe Stromzufuhr, ohne fossile Brennstoffe**.

---

## ⚙️ Funktionsprinzip – Überblick

### ➤ 1. Wasserstofffreisetzung  
- Verwendung von **MgH₂ (Magnesiumhydrid)**  
- Reaktion: endotherme Dehydrierung bei ca. 300–400 °C  
- In sicherer Form: gepresste Kartusche oder keramisch eingebettet (kein loses Pulver!!)

### ➤ 2. Sauerstoffbereitstellung  
- Verwendung von **CuO (Kupfer(II)-oxid)**  
- Abgabe von O₂ bei ca. 900–1000 °C  
- Passive Regeneration durch Luftzufuhr (Luftfensterkonzept)

### ➤ 3. Reaktionskammer  
- Exotherme Reaktion: H₂ + O₂ → H₂O  
- Temperatur bis zu 1000 °C  
- Komplett geschlossen, ohne offene Flamme, nur katalytisch

### ➤ 4. Wärmerückführung  
- Brennkammer versorgt MgH₂- und CuO-Module thermisch  
- Ermöglicht autothermen Dauerbetrieb ohne externe Heizquelle

### ➤ 5. Energiegewinnung  
- Nutzung von **TEGs (Thermoelektrischen Generatoren)**  
- Umwandlung der Temperaturdifferenz in elektrischen Strom  
- Skalierung durch Anzahl + Positionierung der TEGs

---

##✅ Technische Realisierbarkeit – Kurzfazit
Das Reaktorkonzept ist chemisch und physikalisch vollständig realisierbar.
Alle eingesetzten Prozesse – von der thermischen Wasserstofffreisetzung über die Sauerstoffabgabe aus CuO bis hin zur flammenlosen Reaktion in der Brennkammer – sind wissenschaftlich belegt und technisch umsetzbar.

Die Herausforderung liegt in der thermischen Steuerung und Modulkopplung:

MgH₂ benötigt ~300–400 °C zur H₂-Freisetzung

CuO gibt O₂ erst bei ~900–1000 °C ab

Die Brennkammer muss heiß genug sein, um die Reaktion flammenlos katalytisch zu starten

Wasserdampf muss sicher abgeführt werden, ohne das MgH₂-Modul zu gefährden

Mit geeigneter Isolierung, passiver Wärmeführung und Trennung der Module ist das System prinzipiell baubar.
Das Konzept ist realistisch – aber anspruchsvoll.
Ein sorgfältiger Prototypenbau ist notwendig, aber keine unlösbare Aufgabe.

---

## 🔐 Sicherheitskonzept

- Keine Gase in Tanks → Wasserstoff & Sauerstoff werden **on demand** erzeugt
- Kein Wasserkontakt mit MgH₂ → nur Hitze aktiviert das Modul
- Keine Flamme → katalytisch, kontrolliert, festkörperbasiert
- Luftfenster zur O₂-Regeneration nur passiv geöffnet
- Thermisch isolierte Trennschichten + Sicherheitsblock

---

## 🧱 Modulstruktur (geplant)

| Modul              | Funktion                                        |
|--------------------|-------------------------------------------------|
| MgH₂-Modul         | Wasserstoffquelle (austauschbar oder regenerierbar)  
| CuO-Modul          | Sauerstoffquelle (regenerierbar mit Luft)  
| Brennkammer        | Hauptreaktion H₂ + O₂ → H₂O + Hitze  
| Wärmerückführung   | Passive Wärmeleitung zur Modulversorgung  
| TEG-Einheit        | Stromgewinnung aus Temperaturdifferenz  
| Isolationskern     | Trennung, Hitzeschild, Schutzfunktion  
| Dampfausleitung    | Keine Rückführung von Wasser → Abführung über Keramikauslass  
| Regenerationsmodul (optional) | SOEC-Zelle zur Rückgewinnung von MgH₂ und CuO  

---

## 🔬 Materialien & Bezugsquellen

| Material         | Status / Quelle                      |
|------------------|----------------------------------------|
| MgH₂             | Spezialhandel – nur in fester Form verwenden  
| CuO              | Laborglasversand, Amazon, Fachhandel  
| TEG-Module       | Bi₂Te₃-Basis, z. B. von TEGway, Hi-Z, eBay , DiY
| Gehäusematerial  | Edelstahl / Aluminium (je nach Prototypgröße)  
| Isolation        | Aerogelplatten, Keramik, Schamotte  

---

## 📐 Geplante Ausbaustufen

| Variante              | Zielgröße             | Leistung (geschätzt) |
|------------------------|------------------------|------------------------|
| Mini-Prototyp          | < 20 × 20 × 20 cm       | 2–5 W (z. B. Handy laden)  
| Koffer-Reaktor         | 60 × 40 × 40 cm         | 200–500 W (je nach TEGs)  
| Vollausbau             | < 1 m³                 | 2–4 kW (Hausversorgung)  
| Voll abspacken         | < 20 m³                 | 40–80 kW (klein industrie) (is am ende nur ein "heizungsraum" in der größenordnung)

---

## 📦 Veröffentlichungen & Schutz

- ✅ Lizenz: **CC BY-NC-SA 4.0**  
- ✅ Erstveröffentlichung via [archive.org](https://archive.org/details/trf-rg-w)  
- ✅ GitHub-Repo mit Projektstruktur und ReadMe  
- ✅ Ziel: Schutz vor Patentierung durch Konzerne – Offenlegung sichert Freiheit

---

## 🧠 Technisches Konzept vs. Realität

| Thema                   | Umgesetzt / geplant       |
|-------------------------|---------------------------|
| Theoriekonzept          | ✅ Ausgearbeitet  
| Visualisierungen        | ❌ Explosionsdarstellung, Schnittzeichnung  
| CAD-Modelle             | ❌ Noch nicht funktionierend (hab absolut keine ahnung davon) 
| Mini-Prototyp           | ❌ In Planung  
| Materialbeschaffung     | 🕐 MgH₂-Anfrage läuft  
| Thermosimulation        | 🕐 Noch offen (gute programme sind sehr teuer)
| Veröffentlichung        | ✅ Archiv, GitHub, Reddit  

---

## 🔁 Regeneration – geplantes Prinzip

- MgH₂ wird durch kontrollierte externe Elektrolyse regeneriert (später durch TEG oder Solar gespeist)
- CuO regeneriert sich passiv durch kontrollierten Luftkontakt (poröse Keramiköffnung)
- Entstehendes Wasser wird abgeführt – **nicht** rückgeführt 

---


