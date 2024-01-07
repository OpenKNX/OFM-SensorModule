### **Kalibrierungsfortschritt ausgeben**


Manche Sensoren benötigen eine Kalibrierung, bevor sie zuverlässige Werte ausgeben können. Dies ist besonders für die Erfassung von Voc-Werten notwendig. Das Sensormodul hat für den BME680 eine Selbstkalibrierung implementiert, die ununterbrochen parallel zur Messwerterfassung läuft und die bisher ermittelten Kalibrierungswerte in den nichtflüchtigen Speicher des Prozessors speichert. Somit wird verhindert, dass nach einem Neustart des Gerätes eine erneute Kalibrierung notwendig wird.

Bei einer Erstinbetriebnahme, nach dem Einspielen einen neuen Firmware oder in seltenen Fällen auch im normalen Betrieb ist es notwendig, dass sich der Sensor BME680 neu kalibriert. Dies ist daran zu erkennen, dass der Sensor für den Voc-Wert konstant eine 25 liefert und als Kalibrierungsfortschritt über das KO 24 der Wert 0% geliefert wird.

Nach ca. 5 Minuten werden die ersten Voc-Werte ungleich 25 geliefert mit einem Kalibrierungsfortschritt von 33%. Diese ersten Werte sind noch immer nicht sinnvoll zu verwenden.

Nach einiger Zeit (hängt von der Raumgröße, Luftqualität, Lüftungszustand etc. ab) geht der Kalibrierungsfortschritt auf 66%, gefolgt von einem Wert von 100%. Dies kann insgesamt 6 bis 48 Stunden dauern und entspricht einer normalen Funktion des BME680.

Der Kalibrierungsfortschritt kann mit dieser Einstellung zur Information über KO 24 ausgegeben werden, hat aber auf die Funktion keinerlei Einfluss.

