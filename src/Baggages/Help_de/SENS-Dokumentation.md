### Dokumentation


Eine vollständige Applikationsbeschreibung ist unter folgendem Link verfügbar: https://github.com/OpenKNX/OFM-SensorModule/blob/v1/doc/Applikationsbeschreibung-Sensor.md

Weitere Produktinformationen sind in unserem Wiki verfügbar: https://github.com/OpenKNX/OpenKNX/wiki/Produktinfo-Sensormodul


Das Sensormodul erlaubt die Ausgabe verschiedener Sensorwerte auf den Bus. Dabei werden die in KNX üblichen Manipulationen der Sensorwerte unterstützt. Unterstützt werden:

* Sensoren zur

  * Temperaturmessung
  * Luftfeuchtemessung
  * Luftdruckmessung
  * VOC-Messung
  * CO2-Messung
  * Helligkeitsmessung
  * Entfernungsmessung

* Konfigurationen
 
  * Messwert anpassen (verschieben um einen positiven oder negativen Wert)
  * bis zu 2 weitere Messwerte berücksichtigen (Mittelwertbildung mit frei einstellbaren Anteilen pro Messwert)
  * zyklisch Senden
  * bei absoluter Abweichung senden
  * bei relativer (prozentueller) Abweichung senden
  * Messwert glätten

* Abgeleitete (berechnete) Messwerte

  * Taupunkt (wenn Temperatur und Luftfeuchte gegeben ist)
  * Behaglichkeit (abgeleitet aus Temperatur und Luftfeuchte)
  * Luftgüte (aus VOC- oder CO2 abgeleitet)

* Sensorspezifische Zusatzfunktionen

Weitere KNX-Übliche Funktionen wie Schwellwertschalter, Hystereseschalter, auch mit über den Bus einstellbaren Schwellwerten, können über das beiliegende Logikmodul einfach abgebildet werden.

