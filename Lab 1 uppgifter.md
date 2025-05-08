# Förberedelseuppgifter
1. Första uppgiften
	1. $V_{fs}$ = $3.3V - 0V = 3.3V$
	2. $V_{lsb} = \frac{3.3V}{4095} = 0.8mV$
2. Vi antar att vi försöker minimera avrundningsfelet för pga trunkering. Vi konverterar också från $[0, 3.3V]$ till $[0, 4095]$.
	1. $k_0$ är då för konverteringen, alltså måste den vara $V_{lsb}^{-1}$ alltså $\frac{4095}{3.3V}$
	2. $m_0$ är för att minimera avrundningsfel för trunkering. Vi vill alltså efterlikna avrundning. Då är $m_0 = 0.5$ (kanske ska subtrahera m0 med 2048, om vi ska konvertera till )

# Actual lab
- 1.2.3.1 [1240, -1241]
- 1.2.3.2 [1277, -1244] lite fel o brus
- 1233 ~~Använd uträkningen men sätt z till upmätta värdena från socilloskopet
	- $z*k_0 + m_0 = [1277, -1244]$ ger $k=1255, m = 2060,55$ 
- 1234 $20\cdot\log\left(\frac{1}{\sqrt{2}}\right)=-3.010299957$, vilket matchar vad vi såg 
- 1235 $1.642V$
- 1241 vi ser 10 steg. Ganska vettigt eftersom 4 bit ger max 15. $\frac{1277}{2048} \approx 0.62$      $16*0.62 \approx 9.97$
	- Vi ser med lite mindre än två trappsteg per 500 tidigare trappsteg alltså $500\cdot k_{0}^{-1} \approx 0.40 V$ 
- 1242 Alls värden avrundas nedåt, vilket ger en nivå mindre ($2048/16 = 128$) vilket matchar vad vi såg med -127
- 1243 när du rundar nedåt till en en nivå, kan den spendera olika nivå på olika nivåer när derivatan av kurvan ändras
- 1244 Ljudet blir brusigare och verkar få högre tonhöjd vid lägre upplösning.
- 1245 Med lägre upplösning får man mer brus.
	- När kurvan blir kantigare behöver man fler sinuskurvor med olika frekvenser för att approximera denna stegkurva. Dessa dyker up som extra frekvenstoppar.
- 1246 Med fyra bitar går det att uppfatta med svårighet. Med två bitar går det inte att tolka.
- 1251 Denna gången är det bredden (tidsupplösningen) som begränsar trappstegen, alltså är bredden samma, medan höjden varierar. 
	- Uppmätt längd på steg är ungefär 3 steg på 1 ms ger $\frac{3}{1\cdot10^{3}} = 0.003 s/steg$
	- Teoretisk längd på steg: $4kHz$ ger $\left(4000\right)^{-1} = 2.5ms/steg$ , ungefär samma
- 1252 ingen stor skillnad i ljudet 
- 1253 Det låter mörkare. Toppen finns på 621 hz. Anledningen är att samplingsfrekvensen är under halva insignalsfrekvensen. This leads to aliasing.
- 1254 Med "banan banan" märkte vi skillnad först vid 4kHz. 2kHz låter väldigt annorlunda. 1kHz är lite cooked.
- 1255 Vågen låter bra vid 32kHz, lite sämre vid 16kHz, och helt annorlunda på lägre sampling rate. Anledningen till att denna på värkas mer än en sinusvåg är förmodligen att om man missar vägen med mycket i samplingen är det värre än med en sinusvåg där man hela tiden fångar små förändringar.
	- 1/3 är -4.77 dB och -9.54 i dBV skalan

| peak (n) | förväntad freq () | uppmätt freq () |
| -------- | ----------------- | --------------- |
| 1        | 440               | 440             |
| 3        | 1320              | 1320            |
| 5        | 2200              | 2200            |
| 7        | 3080              | 3077            |
| 9        | 3960              | 3957            |
| 11       |  4840             | utanför         |

- 1261 $a_{500} = 0.385$ $a_{520} = 0.410$ $\Delta a =  0.025$ den förväntade skillnaden är $20\cdot1255^{-1} \approx 0.0159$ skillnaden är ungefär $9mV$
- 1262 vi gjorde om mätningarna och fick $a_{500} = 0.390$ $a_{520} = 0.410$  $\Delta a =  0.020$ och detta stämmer med den nya förväntade skillnaden när man tänker på buggen: $26\cdot1255^{-1} \approx  0.021$
- 1263 Man ser den, se bilden. Man ser en extra lång platt nivå, eftersom den nivån motsvarar fler amplituder.