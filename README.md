# EVOpt Home Assistant Addon

Dieses Home Assistant Addon bietet eine bequeme Möglichkeit, die [EVOpt](https://github.com/andig/evopt)-Lösung lokal als Addon in Home Assistant zu betreiben. EVOpt ist eine Optimierungslösung für das Laden von Elektrofahrzeugen, die in Kombination mit [evcc.io/evcc](https://github.com/evcc-io/evcc) verwendet werden kann.

---

## Über EVOpt

EVOpt ist eine Software, um intelligentes, dynamisches Laden von Elektrofahrzeugen basierend auf verschiedenen Parametern, einschließlich Energiepreisen, Verfügbarkeiten und Ladebedarfen, zu optimieren. 

Die Kombination mit [evcc.io/evcc](https://github.com/evcc-io/evcc) ermöglicht das simple und effiziente Management der Ladeinfrastruktur.

---

## Features

- Integration in Home Assistant als eigenständiges Addon
- Optimierung der Ladezeiten und -mengen für Elektrofahrzeuge
- Nutzung von Daten und Steuerfunktionen von evcc
- Automatische Anpassung an variable Stromtarife und Energieflüsse

---

## Installation

1. Füge das EVOpt Addon-Repository in Home Assistant hinzu:

   Repository URL:
   ```
   https://github.com/thecem/hassio-evopt
   ```

2. Suche in der Addon-Liste nach "EVOpt" und installiere das Addon.

3. Konfiguriere das Addon über das Home Assistant Addon Panel (siehe Konfiguration unten).

4. Starte das Addon.

---

## Konfiguration

Die Konfiguration erfolgt über die `config`-Sektion des Addons, z.B. in der `options`:

```
# Beispiel-Konfiguration (anpassen nach Bedarf)
evcc_api_url: "http://localhost:7070/api"  # URL zur evcc API
charging_mode: "optimiert"                 # Beispiel-Parameter
max_current: 16                            # Maximale Stromstärke in Ampere
tariffs:
  - "tag"
  - "nacht"
```

Für eine vollständige Beschreibung der Parameter und deren Bedeutung empfiehlt sich die Lektüre der evcc-Dokumentation unter:  
[https://github.com/evopt/evopt](https://github.com/andig/evopt)

---

## Verwendung

Nach der Konfiguration und dem Start des Addons kommuniziert EVOpt mit evcc, um Ladeprofile für Elektrofahrzeuge optimal zu steuern. Die Steuerung erfolgt automatisch und passt sich an Deine individuellen Anforderungen und Stromtarife an.

---

## Links
- evopt Repository: [https://github.com/andig/evopt](https://github.com/andig/evopt)
- EVOpt Repository: [https://github.com/thecem/hassio-evopt](https://github.com/thecem/hassio-evopt)
- evcc Repository: [https://github.com/evcc-io/evcc](https://github.com/evcc-io/evcc)

---

## Disccussion

https://github.com/evcc-io/evcc/discussions/

---

## Support & Mitwirkung

Für Support, Fragen oder Beiträge zum Projekt besuche bitte das Repository und öffne gegebenenfalls Issues oder Pull Requests.

---

## Lizenz

Informationen zur Lizenz des Addons sind im Repository zu finden.

---

*Dieses Addon ist eine Ergänzung zur evcc-Projektlösung für intelligente Elektrofahrzeugladeoptimierung in Home Assistant.*
