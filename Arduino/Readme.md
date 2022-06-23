# Arduino-Code

Hinweise zum Flashen:

Ich habe zum Flashen die Arduino IDE mit der Board Erweiterung 
"MiniCore" benutzt. Die erlaubt das Flashen ohne bootloader dierekt über 
den ICSP header. Eigentlich wollte ich ein volles flashen über den USB 
mit dem Arduino bootloader ermöglichen, aber da ist leider ein kleiner 
desing bug auf dem PCB.
Ich habe vergessen die RST leitung vom ATMEGA über einen 0.1uF 
Kondensator mit dem DTR vom CP2102 zu verbinden. Ich würde dir auch 
empfehlen falls du das PCB bearbeiten solltest auch 3.3V TVS Dioden an 
den vorgesehenen stellen auszulöten.
