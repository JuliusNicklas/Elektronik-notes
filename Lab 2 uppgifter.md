2.1.2.2
$$
20\cdot\log\left(\frac{\frac{\frac{1}{k}\sin\left(k2\pi440\cdot\frac{\pi}{2}\right)}{\sqrt{2}}}{1}\right)-20\cdot\log\left(\frac{\frac{\sin\left(2\pi440\cdot\frac{\pi}{2}\right)}{\sqrt{2}}}{1}\right)
$$
kanske:

$$
20\cdot\log\left(\frac{\frac{\frac{4}{\pi}\frac{1}{k}\sin\left(k2\pi440\cdot\frac{\pi}{2}\right)}{\sqrt{2}}}{1}\right)-20\cdot\log\left(\frac{\frac{\frac{4}{\pi}\sin\left(2\pi440\cdot\frac{\pi}{2}\right)}{\sqrt{2}}}{1}\right)
$$

kan förenklas till $20 \cdot log\frac {1}{k} = -20logk$

Dämpning:
$$
D_{k}=1\cdot\frac{1}{\sqrt{1+\left(2\pi440kRC\right)^{2}}}
$$
Kan förenklas till:
$$
-10\log\left(1+\left(2\pi\cdot440k\cdot RC\right)^{2}\right)
$$
# 2.2.1
### 2.2.1.1
Peakarna är mycket högre och tydligare med en högre sample rate. De aliasade frekvenserna förstärker inte varandra lika mycket, så de blir lägre. Kort sagt mycket tydligare och bättre. Man ser vilka frekvenser som hör hemma.

### 2.2.1.2

$32000-k\cdot440$ ger att första speglingen in (och därmed den största) är $k = 65$ alltså $\kappa = 65$

### 2.2.1.3
$f_\kappa = 65 \cdot 440 = 28600$
$f_K = 32000-f_\kappa = 3400$

### 2.2.1.4
med formel för dämpning (från uppgift 2.1.2.2) $20 \cdot log\frac {1}{k}$ får vi att dämpningen av $\kappa$ är $-36.26dB$
Det uppmätta värdet är ungefär $37.1dB$, vilket stämmer ganska bra med det teoretiska

### 2.2.1.5 
Se 2.2.1.4

# 2.2.2

### 2.2.2.1
Allt ovanför 4kHz är nästan noll, eftersom det är ett filter för sampling rate på 8kHz.

De speglade frekvenserna påverkas inte så mycket eftersom det är ett digitalt filter, och man behöver ett församplingsfilter, alltså ett analogt filter för att ta bort dem.

### 2.2.2.2
ungefär $-38.0dB$, vilket är bara "en tjugondels 10 gånger mindre". Alltså inte så stor skillnad, eftersom den är inspeglad
Note: skriv sen invers decibelformel av -1

# 2.2.3

### 2.2.3.1
ungefär $-38.1dB$, basically ingen skillnad

# 2.2.4

Nu ser man tydligt att signaler som speglas från längre och längre bort får lägre och lägre amplitud. Man kan skilja på "första ordningens och andra ordningens" spegling.
### 2.2.4.1
amplituden av $f_\kappa$ är nu $-53.9dB$ en stor förbättring. 

### 2.2.4.2
amplitud av$f_\kappa$ är $B_\kappa + D_\kappa = -20log(\kappa) + -10log(1+(2\pi 440\kappa \cdot RC )^2) = -51.6dB$ Detta är ganska nära det uppmätta värdet.

# 2.2.5

### 2.2.5.1
amplituden av $f_\kappa$ är nu $-69.5dB$ en stor förbättring. 

### 2.2.5.2
Av bode-diagrammet läser vi av ungefär $-35dB$ för 28600Hz
amplitud av$f_\kappa$ är $B_\kappa + D_\kappa = -20log(\kappa) + -35 = -71.3dB$ Detta är ganska nära det uppmätta värdet.

# 2.2.6

### 2.2.6.1
Det ser smegsigt ut och precis som i våra våtaste drömmar.

2.2



