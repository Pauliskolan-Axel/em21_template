# em21_template

Projekt 1: Solcellsdriven WiFi-sensor

Detta projekt kräver en del lödning som också kommer ta tid. Laddare, INA, OLED etc.
Du ska skicka data till en grupp på min AIO-sida. Detaljer senare.

E:	Skicka data från uppladdningen, spänning, fuel gauge, temp etc. 
	Sleep fixed time (kolla ESP32 exempel). Använd adafruitio_11_group_pub. 
	Löda laddare/termistor.
D:	OLED med auto-off, initiera med Reset. Stäng av laddning om termistorn varnar. 
	Avbryta Wifi om man inte får kontakt. Löda OLED.
C:	INA219 laddningsmätare, touch wake up med OLED från D. Versionskontroll via 
	Github. Justera/avbryta uppdatering m.a.p. batteriprocent. Skicka mejl om
	batteriet understiger viss nivå via IFTT.
	Löda INA/doubler.
B:	OLED med knappstyrd presentation (med font) av data, skicka data med 
	konstant interval med sleep (trots ev knapptryck), dokumentering av 
	insamlad data.. Skjuta ner periferials och wifi innan sleep, se länkar i classroom.
A:	Försök att mäta antalet blink i laddningskretsen med external wake up, skicka 
	meddelande på valfritt sätt med batterivarning.
	Analys av data och korrigering av sleep time m.a.p. hur mycket procent av
	batteriet är kvar (wake up stub, ISR).
	
Här är en lista på de “Issues” du ska skapa i ditt repo på Github:
Varje Issue får ett nummer som du använder i VS code när du commit:ar)

[Feature] Skjuta ner s.k. periferials och wifi innan sleep enhancement
[Feature] Konstant uppdatering, trots knapptryck enhancement
[Feature] OLED flera menyer enhancement
Löda INA219
[Feature] Skicka meddelande om batteriet understiger viss nivå enhancement
[Feature] Variabel sleep time map batteriprocent enhancement
[Feature] INA219 laddningsmätare enhancement
[Feature] Avbryt WiFi om du inte får kontakt enhancement
Löda OLED
[Feature] Stäng av laddning om temperaturen är för hög enhancement
[Feature] OLED enhancement
[Feature] Sleep fixed time, send fuel gauge data to AIO. enhancement
Löda laddare
	
	

