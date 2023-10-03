# Opdracht 1 
Schrijf een programma dat 2 getallen als gebruikersinput krijgt. Verwissel de variabelen van positie. 

Voorbeeld: getal1 = 10, getal2 = 20
Resultaat: getal1 = 20, getal2 = 10

Tip gebruik een derde variabele als tussenstap. 

# Opdracht 2 
Het is het einde van de lesperiode. Schrijf een programma waarin je jouw cijfers voor de vakken Nederlands, Engels en rekenen in kan voeren. Het programma print vervolgens het gemiddelde cijfer in de console. 

Schrijf een programma dat: 
1. 3 cijfers leest vanaf de console en opslaat in een variabele (cijfers kunnen decimale getallen zijn tussen de 1 en 10)
2. Het gemiddelde berekend van de ingevoerde cijfers
3. Het gemiddelde cijfer in de console print op 1 decimaal nauwkeurig. 

Voorbeeld: Nederlands 6.5, Engels 7,2; rekenen 4,7
Resultaat: "Het gemiddelde cijfer is een 6.1"

# Opdracht 3
Maak het programma in de vorige opdracht opnieuw. Zorg dat het programma opmerking geeft over het behaalde cijfer. 

|-|-|-|-|
| Cijfer >= 8,0 | "zeer goed gedaan!" |
| Cijfer >= 6,0 && Cijfer < 8,0 | "keurig!" | 
| Cijfer >= 5,5 && Cijfer < 6,0 | "net voldoende." |
| Cijfer >= 4,0 && Cijfer < 5,5 | "dat is niet goed genoeg." |
| Cijfer < 4 | "Gezakt!" |

Voorbeeld: Nederlands 6.5, Engels 7,2; rekenen 4,7
Resultaat: "Het gemiddelde cijfer is een 6.1, keurig!" 

Voorbeeld2: Nederlands 4.2, Engels 5.8; rekenen 3,1 
Resultaat: "Het gemiddelde cijfer is een 4.3, dat is niet goed genoeg."

# Opdracht 4
Maak een uitbreiding op het programma uit opdracht 2. Je hebt natuurlijk meer vakken dan Nederlands, Engels en Rekenen. 

Zorg dat het programma aan de gebruiker blijft vragen of hij nog een cijfer in wil voeren. Pas als de gebruiker "nee" invult berekent het programma het gemiddelde van alle ingevoerde cijfers. Maak hiervoor gebruik van een while loop. Het is niet nodig ieder cijfer in een aparte variabele op te slaan.

Schrijf een programma dat:
1. De gebruiker vraagt een cijfer in te voeren. Tel het cijfer op in een variabele. Denk eraan een counter bij te houden.
3. De gebruiker vraagt of hij nog een cijfer in wil voeren.
4. Loop stap 1 en 2 tot de gebruiker "nee" invoert.
5. Print het gemiddelde en de opmerking op de console

Voorbeeld, gebruikers input: 8.3, 6.2, 4.1, 9.4, 4.0 
Resultaat: "Het gemiddelde is een 6.4, keurig"

# Opdracht 5
Je hebt een bitcoin gekocht en de prijs fluctueert sterk. Maak een programma die als input de aankoopprijs en het percentage verandering krijg. Bereken de nieuwe waarde en het prijsverschil. 

Schrijf een programma dat:
1. De gebruiker om de aankoopwaarde vraagt en sla die op in een variabele
2. De gebruiker om het procentuele prijsverschil vraagt
3. Print in de console de nieuwe prijs en het prijsverschil in euro's

Voorbeeld: aankoopprijs €10.000 en percentage 10%
Resultaat: de huidige prijs is €11.000 en het prijsverschil is €1000


# Opdracht 6 
Schrijf de functie `oppervlakteRechthoek(int lengte,  int breedte)`.  In de functie wordt het oppervlakte van het rechthoek berekent. Het oppervlakte is de `return` waarde van deze functie. 

### Voorbeelden C#
```
Console.WriteLine($"Oppervlakte is: {oppervlakteRechthoek(10, 10}")) //output Oppervlakte is: 100
Console.WriteLine($"Oppervlakte is: {oppervlakteRechthoek(25, 5}")) //output Oppervlakte is: 125
Console.WriteLine($"Oppervlakte is: {oppervlakteRechthoek(3, 3}")) //output Oppervlakte is: 9
```


# Opdracht 7
Je hebt vast 3 producten die je vaak koopt bij de supermarkt waarschijnlijk: energieblikje, frikandelbroodjes en pringles. Je wil vast regelmatig weten hoeveel van deze items je nog kan kopen met het bedrag op je rekening. *Let op je kunt natuurlijk geen half frikandelbroodje kopen of 3/4 blikje energiedrink*

Schrijf een programma dat: 
1. Vraagt hoeveel geld je in totaal nog hebt
2. Vraagt wat de prijs is van een energieblikje, frikandelbroodje en pringles
3. Print in de console hoeveel je van ieder item kan kopen.  

Voorbeeld: geld = 10, energieblikje = 1, frikandelbroodje = 2, pringles = 3
Resultaat: "Met €10 kun je 10 energieblikjes, 5 frikandelbroodjes of 3 bussen pringles kopen"


# Opdracht 8
Schrijf twee functies `inclBTW(double prijs, int percentage)` en `exclBTW(double prijs, int percentage)`

Functie 1 berekent de prijs inclusief btw en geeft dit als return waarde.  
Functie 2 berekent de prijs exclusief btw en geeft dit terug als returnwaarde. 

Gebruik voor functie 1 de volgende formule:
$$
inclBTW = prijs *  (1 + \frac{percentage} {100})
$$ 

Gebruik voor functie 2 de volgende formule: 
$$
exclBTW = prijs -  (( \frac{percentage} {(100 + percentage)}) * percentage)
$$ 

### Voorbeelden C#
```
Console.WriteLine($"bedrag inclusief BTW is: €{inclBTW(100, 9}" // output: bedrag inclusief BTW is: €109
Console.WriteLine($"bedrag exclusief BTW is: €{exclBTW(100, 21}" // output: bedrag exclusief BTW is: €82,64
```

# Opdracht 9
Met de meeste operators (+, -, \*, / ) ben je wel bekent. In het programmeren wordt ook gebruik gemaakt van de module operator (%). De module geeft de restwaarde nadat het linker getal door het rechter getal gedeeld is.

**Voorbeelden**
1 % 3 = 1
2 % 3 = 2
3 % 3 = 0
4 % 3 = 1 
5 % 3 = 2 
6 % 3 = 0 

Met de modulo kunnen we, nu, twee leuke trucjes toepassen. 
evengetal % 2 = altijd 0 (dus 123456 % 2 = 0)
getal  % 10 = laatste getal van de int. (dus 123456 % 10 = 6)

Schrijf twee functies 
`bool even (int getal)` en `int laatsteGetal(int nummer)`

De functie even heeft de return waarde True als het getal even is en False als getal oneven is. 
De functie laatsteGetal heeft als return waarde het laatste getal van het ingevoerde nummer

#### Voorbeelden 
```
Console.WriteLine(even(1564)); // True
Console.WriteLine(even(45641)); // False
Console.WriteLine(even(4896465)); // False

Console.WriteLine(laatsteGetal(1564)); // 4
Console.WriteLine(laatsteGetal(45641)); // 1
Console.WriteLine(laatsteGetal(4896465)); // 5
```

# Opdracht 10
Vraag de gebruiker hoeveel uren hij deze week aan Gamen, Social Media en  huiswerk heeft besteed.

Als het totaal totaal meer dan 110 uur is print in de console: "Zo hee hoef jij niet te slapen?"
Als het meeste uren besteed wordt aan:
Gamen - print in de console: "Huiswerk is belangrijker dan gamen!"
Social Media - print in de console: "Minder tiktok meer programmeren!"
Huiswerk - print in de console: "Dan zul je wel goede cijfers halen!"

Voorbeeld: gamen = 40, socialMedia = 20, huiswerk = 2
Output: "Huiswerk is belangrijker dan gamen!"

Voorbeeld: gamen = 50, socialMedia = 60, huiswerk = 5
Output: "Zo hee hoef jij niet te slapen?"

# Opdracht 11
In de bibliotheek kun je gebruik maken van privé studieruimtes. Als je lid bent van de bibliotheek betaal je €2/uur voor deze ruimte. Niet leden betalen €5/uur voor deze ruimte. Als de ruimte langer dan 3 uur door 1 persoon gebruikt wordt krijgt deze persoon 20% korting.

Schrijft een programma dat:
1. Vraagt en opslaat hoe lang de ruimte is gebruikt.
2. Checkt of de ruimte is gebruikt door een lid
3. Bepaald of de gebruiker korting krijgt.
4. Print hoeveel de gebruiker moet betalen

Voorbeeld: uren = 4, lid = nee
Output: "De gebruiker is geen lid, heeft de ruimte 4 uur gebruikt voor €5 per uur. De gebruiker krijgt wel 20% korting. De totaalprijs is €16."

**Formule om **
$$
kortingsprijs = verkoopprijs -   \frac{verkoopprijs} {100} * kortingspercentage) 
$$

Voorbeeld: Als je 15% korting krijgt en de oorspronkelijke prijs € 85 is, kunnen we de formule als volgt invullen: € 85 - (€ 85 / 100 * 15%) = € 72,25. Je korting is € 12,75 (€ 85 - € 72,25)

# Opdracht 12
Je wil iets kopen op amazon.de. De verkoper rekent de volgende verzendkosten: 
Duitsland €3
Nederland €5 
België €7
Alle andere landen €9.

Schrijf een programma dat:
1. Vraagt wat de kosten van het product zijn
2. Naar welk land het moet worden verzonden
3. Print wat de verzendkosten zijn en het totaal bedrag is dat moet worden betaald.

Voorbeelddata: prijs = 50, land = Zweden
Output: "Het totaalbedrag is €59, €50 voor het product en €9 verzendkosten."

# Opdracht 13
Een telefoonbedrijf rekent de volgende maandelijkse kosten voor

**Vaste kosten: €25 (aansluitkosten)**
**Variabele kosten volgens onderstaande tabel:** 
| Bel tijd in seconden | Kosten in € per seconde |
|---------|--------------|
| 1-500 | 0,01 |
| 501-800 | 0,008 |
| 801+ | 0,005 |


Schrijf een programma dat:
1. Vraag hoeveel seconden er deze maand zijn gebeld
2. De kosten voor deze maand berekent 
3. De kosten in de console print.

Resultaat: "Totale kosten deze maand: €48"

#### Let op! De kosten voor de eerste 500 seconden zijn altijd €0,01 dan voor alle seconden tussen 501 en 800 zijn de kosten €0,008 en voor alle seconden meer dan 801 €0,005 
