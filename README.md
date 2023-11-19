# STM32-Projekat-blinkanje-LED-diode-sa-Proteus-Simulacijom
Ovaj projekat ima za cilj demonstraciju osnovnih principa programiranja mikrokontrolera na platformi STM32, kroz jednostavan primer blinkanja LED diode. Kroz projekat, koristićemo STM32CubeIDE, popularno integrisano razvojno okruženje za rad sa STM32 mikrokontrolerima i simulacioni softver Proteus za proveru funkcionalnosti pre učitavanja na stvarni mikrokontroler.

## Detalji projekta
### Odabir porta i pina
Prilikom odabira porta i pina za povezivanje LED diode, koristili smo jednostavna pravila zasnovana na broju i tipu slova sadržanih u imenu studenta koji radi projekat i to na sledeći način: <br />

* if(broj_samoglasnika > broj_suglasnika) <br />
*  PORT = PORTA <br />
* ELSE <br />
*  PORT = PORTB <br />

S obzirom da u imenu  **ANA CVIJOVIĆ** imamo 5 samoglasnika i 6 suglasnika odabran je **PORTB**.

PIN je odabran kao rezultat deljenja broja koji predstavlja zbir slova u imenu i prezimenu po modulu 6. <br />
To u mom primeru predstavlja **11mod6 = 5**, tako da je odabran **PIN_5**.

## Širina impulsa i pauze
Širina impulsa je jednaka dužini imena izraženoj u ms, dok je širina pauze jednaka dužini prezimena izraženoj u ms. Pri ponavljanju se vrednosti rotiraju. <br />
U mom slučaju širina impulsa najpre iznosi **3 ms**, a širina pauze **8 ms**.


## Korišćene tehnologije
**STM32CubeIDE**: IDE za razvoj softvera za STM32 mikrokontrolere. <br />
**Proteus**: Simulacioni softver za proveru funkcionalnosti elektronskih sistema.
