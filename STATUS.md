# STATUS
## BINARY SENSOR: ALARM

### States

The Alarm sensor becomes `ON` (true) when the current phase is:
- `Einmaischen Temp. erreicht` - Mash-in temperature reached
- `Rastende erreicht` - Rest end reached

This matches the alarm states in the Braumeister device and Speidel WebUI.

## CURRENT PHASE
- Prost!
- Jetzt Whirlpool …
- Brauvorgang beendet
- Hopfen kochen
- Rastende erreicht --> ALARM
- 1. Rast
- Einmaischen Temp. erreicht --> ALARM
- Einmaischen
- RECIPENAME starten
- Hauptmenü

## CURRRENT STEP
- Prost!
- Jetzt Whirlpool …
- Brauvorgang beendet
- RECIPENAME – Hopfen kochen
- RECIPENAME - Rastende erreicht --> ALARM
- RECIPENAME – 1. Rast
- RECIPENAME – Einmaischen Temp. erreicht --> ALARM
- RECIPENAME – Einmaischen
- Automatik – RECIPENAME starten
- Hauptmenü

## ALARM WITHOUT OUTPUT in HA
- Deckel entfernen: 
  Target Temperature: 103,0 °C
  Temperature: 100,5 °C
- Hopfengabe

