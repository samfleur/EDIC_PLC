
![logotransparant (1)](https://github.com/samfleur/EDIC_PLC/assets/54836951/230b4d6a-2375-41c1-9a36-6df19019ba99)


## PLCprogramv1

Beginsel, eerste versie

I3 actief → remote

I4 actief → local

geen uitsluiting of iets dergelijks, ook niet van toepassing in theorie. Misschien nog indien geen van beide actief foutmelding?

Als start signaal van winch (I1) & op remote en niet op stop → set start

Analog input 1 (I7) → met een analog amplifier er tussen om te mappen tussen 100 en 1000 → output naar AQ1 (U1+ en M1 (0 tot 10V) (input voor VFD)

Beide schermen actief met een status (local / remote) en de (gewenste) snelheid van de pomp

![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/ebd99798-918e-41fc-b873-9251d1de49f0)

## PLCprogramv2

Selectie van potmeter afhankelijk van status:
Altijd 100, behalve bij status M7, dan snelheid van de potmeter.

Local start en stop.
Selectie van remote en de aangehangen statussen richting winch cabinet.

![image](https://github.com/samfleur/EDIC_PLC/assets/54836951/e72101d0-76ac-4a8a-8b6c-9fa10695ad0b)
