
![logotransparant (1)](https://github.com/samfleur/EDIC_PLC/assets/54836951/230b4d6a-2375-41c1-9a36-6df19019ba99)


## PLCprogramv7

Goedemorgen, bij deze zijn het 4 pagina's geworden.
- Alle scherm updates zijn toegevoegd
- Bij een winch trip gaat ie automatisch naar running en volle snelheid
- Als zowel de static brake en de pomp draaien in remote stopt ie ermee en gaat ie automatisch naar standby

### Local / Remote, Heater toggle, lamp test, trip situations including winch trip, 
![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/1c11e373-c054-43c4-9f6e-c221d83f58b2)
### Display updates
![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/390750f1-bb13-43f6-ac17-78670ee6b2d7)
### Local start / stop, F1 toggle between standby and running, safety trip during running
![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/45435476-5996-4509-8b41-d2ec43b3a336)
### Remote starting / stopping, lowering / hoisting, stopped / standby / running setting and starting of VFD
![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/54723389-73cf-415a-b7ea-a1f50a81d6ce)


## PLCprogramv5

Paar versies verder, vrij succesvol tot nu toe. Oh ja het zijn twee pagina's geworden, is blijkbaar een optie.
To do:
- scherm updates
- lower & static released van winch (iets van set reset op static release en dan moet zodra lower binnen komt de brake van standby naar running)

![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/4595e80d-a31b-4386-95e4-d43a7556de63)
![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/b7a645b8-f697-4328-8757-c9c9b64ed784)


## PLCprogramv2

Selectie van potmeter afhankelijk van status:
Altijd 100, behalve bij status M7, dan snelheid van de potmeter.

Local start en stop.
Selectie van remote en de aangehangen statussen richting winch cabinet.

![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/e72101d0-76ac-4a8a-8b6c-9fa10695ad0b)

## PLCprogramv1

Beginsel, eerste versie

I3 actief → remote

I4 actief → local

geen uitsluiting of iets dergelijks, ook niet van toepassing in theorie. Misschien nog indien geen van beide actief foutmelding?

Als start signaal van winch (I1) & op remote en niet op stop → set start

Analog input 1 (I7) → met een analog amplifier er tussen om te mappen tussen 100 en 1000 → output naar AQ1 (U1+ en M1 (0 tot 10V) (input voor VFD)

Beide schermen actief met een status (local / remote) en de (gewenste) snelheid van de pomp

![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/ebd99798-918e-41fc-b873-9251d1de49f0)

