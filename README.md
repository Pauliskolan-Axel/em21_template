E:	Skicka data från sol-uppladdningen, spänning, fuel gauge, temp etc. 
	Sleep fixed time (kolla ESP32 exempel). Använd adafruitio_11_group_pub. Döp dina feed-group till dina initialer.
	Löda laddare/termistor.
D:	OLED med auto-off, initiera med Reset-knapp.
	Justera/avbryta uppdatering m.a.p. batteriprocent.
	Avbryta Wifi om man inte får kontakt. 
	Löda OLED.
C:	INA219 laddningsmätare, skicka upp strömmen (medelvärde) till AIO. 
	Stäng av laddning om termistorn varnar.  	
	External Wake up med knapp. Visa data på OLED utan att skicka.
	Skicka data med konstant interval med sleep (trots ev. knapptryck).	
	Löda INA/doubler.
B:	OLED med knappstyrd presentation med font. Två knappar/frames.
	Skicka mejl om batteriet understiger viss nivå via IFTT.  
	Dokumentering av insamlad data.
	Versionskontroll via Github (och helst VS code). 
	Skjuta ner s.k.  periferials och wifi innan sleep, se länkar i classroom.
A:	Försök att mäta antalet blink i laddningskretsen med external wake up. 
	Skicka meddelande mha “integrations” till dig, på valfritt sätt (mejl, app, twitter 
	etc) med batterivarning.
	Längre sleep time mellan 18-06 (hämta tid från AIO)
