## Øvinger etter forelesning 23.08.2017

#### Hva er HTML?
HTML er et markeringsspråk som brukes for å strukturere
informasjon, som regel på en webside.

#### Hva er HTML5?
HTML5 er den nyeste versjonen av HTML. Med HTML5 har man
flere muligheter, blant annet mulighet å få tilgang til
midlertidig lagring gjennom locastorage. HTML5 støtter også
egne tagger for multimedia, canvas/svg og flere atributter,
bl.a. range, number, date osv.

#### Hva menes med semantisk koding i HTML
Med semantisk koding menes det at man bruker tagger
slik det er ment til å - og slik det gir mening at de -
brukes. Det handler om at koden er ryddig og fortåelig
for både deg selv (den som skirver) og andre.

#### Hva er forholdet mellom HTML og CSS
HTML brukes for å strukturere/holde selve informasjonen.
CSS kan brukes for å legge til stiler på "topp av" HTML,
slik at det blir pent og slik at man får en behagelig,
intuitiv brukeropplevelse

#### Hva er Doctype-deklarasjonen for?
Doctype-deklarasjonen har som funksjon å fortelle nettleseren hva slags dokument det er. f.eks. vil
"<!doctype html>" fortelle nettleseren at det er
HTML5 den kan forvente i det kommende dokumentet

#### Hvordan er Doctype-deklarasjonen for XHTML 1.0 Strict?
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">  

#### Hvordan er Doctype-deklarasjonen for HTML5?
<!doctype html>

#### Hvilke HTML-tager må minimum være med i et HTML5-dokument?
doctype- og html-tag

#### Hvor mange head-tager (hvor h1 er en av dem) er det?
6 stk.

#### Hva er den korrekte tagen å bruke for å legge til et avsnitt?
< p >< / p >

#### Hvilke deler består en (hyper)lenke-tag av?
en "< li>" og tilsvarende "</ li>", samt en "src=adresse"-atributt

#### Hva er forskjellen mellom ul og ol visuelt?
ul => uordnet liste => kun kulepunkter <br>
   ol => ordnet liste => tall: 1,2,3,4 osv.

#### Hva er forskjellen mellom ul og ol semantisk?
Semantisk gir det mening å bruke ol-tag om det har en funksjon at det man skriver har en spesiell rekkefølge. Tilsvarende gir det ikke mening om det man skal skrive liste over ikke har en bestemt rekkefølge.

#### Lag en tabell for å vise informasjon om ansatte i en bedrift med navn, mobil, stilling og bilde.
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Ansatte</title>
  </head>
  <body>
    <table>
      <tr>
        <th>navn</th>
        <th>mobil</th>
        <th>stilling</th>
        <th>bilde</th>
      </tr>
      <tr>
        <td>Olav</td>
        <td>12345678</td>
        <td>utvikler</td>
        <td>profilbilde_olav.png</td>
      </tr>
      <tr>
        <td>Simen</td>
        <td>98765432</td>
        <td>utvikler</td>
        <td>profilbilde_simen.png</td>
      </tr>
    </table>
  </body>
</html>
```
<head>
  <meta charset="utf-8">
  <title>Ansatte</title>
</head>
<body>
  <table>
    <tr>
      <th>navn</th>
      <th>mobil</th>
      <th>stilling</th>
      <th>bilde</th>
    </tr>
    <tr>
      <td>Olav</td>
      <td>12345678</td>
      <td>utvikler</td>
      <td>profilbilde_olav.png</td>
    </tr>
    <tr>
      <td>Simen</td>
      <td>98765432</td>
      <td>utvikler</td>
      <td>profilbilde_simen.png</td>
    </tr>
  </table>
</body>
#### Hva menes med validering av HTML-kode?
validering gjøres for å sjekke at alt er gyldig.

#### Hva er et attributt? Hva er malen for å legge til et attributt på et element? Ta gjerne utgangspunkt i "a" og "img"
en attributt er en definert egenskap ved et dokument. For
eksempel kan a-tagen ha en "href" attributt som viser til en
annen nettside. Tilsvarende kan "img"-tagen ha en "src" som atributt.

#### Hvilken tag brukes til å legge til et sitat?
```html
<q cite="Olav">Alle jobber</q>
```
<q cite="Olav">Alle jobber</q>
#### Hva er hr-tagen for?
Brukes for å vise at det er en endring i innholdet. I praksis arter den seg i form av en strek på tvers av siden.
```html
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
    </head>
    <body>
      <p>innhold om tema 1</p>
      <hr><!--Her er <hr> -->
      <p>innhold om tema 2</p>
    </body>
  </html>
```
<p> innhold om tema 1
<hr>
<p> innhold om tema 2

#### Hva er br-tagen for?
Br viser et linjeskift i teksten.
```html
  <p>Dette er en tekst <br> med linjeskift</p>
```
<p> Dette er en tekst <br> med linjeskift

#### Hva brukes span-tagen til?
Span brukes til å markere et spesielt område slik at du kan få tilgang til det uten å nødnvendigvis få tilgang til andre ting.

#### Lag et eksempel på bruk av dl-tagen
```html
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
    </head>
    <body>
      <dl>
        <dt>fakta</dt>
        <dd>noe man vil forholde seg til</dd>
        <dt>oppspinn</dt>
        <dd>noe man ikke ønsker</dd>
      </dl>
    </body>
  </html>
```
<dl>
  <dt>fakta</dt>
  <dd>noe man vil forholde seg til</dd>
  <dt>oppspinn</dt>
  <dd>noe man ikke ønsker</dd>
</dl>
Dette er en deskripitiv liste. dl-tage gir altså elementer i en liste, med hver sin beskrivelse.

#### Hvordan åpner man opp en lenke i ny fane eller nytt vindu?

```html
  <!--åpner angitt adresse i samme fane-->
  <a href="https://github.com/">github</a>
  <!--åpner angitt adresse i en ny fane-->
  <a href="https://github.com/" target="_blank">github</a>
```

#### Hvordan legger man til kommentar i koden (som ikke vil være synlig på nettsiden)?
```html
  <!-- slik legger man til kommentarer -->
  <!-- altså mellom disse to forskjellige tegnkomboene -->
```

#### Hva er den korrekte måten å kode opp en navigasjonsmeny?
Lister er den korrekte måten å lage navigasjonsmenyer på, ifølge forelesning.
```html
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
    </head>
    <body>
      <ul> <!-- "hovedmeny" -->
        <li><a href="#datamaskiner">datamaskiner</a></li>
        <ul> <!-- undermeny -->
          <li><a href="#mac">mac</a></li>
          <li><a href="#windows">windows</a></li>
        </ul>
        <li><a href="#klaer">Klær</a></li>
        <ul> <!-- undermeny -->
          <li><a href="#t_skjorte">t-skjorte</a></li>
          <li><a href="#bukse">Bukse</a></li>
        </ul>
        <!-- element under har ikke undermeny -->
        <li><a href="#kontakt">Kontakt</a></li>
      </ul>
    </body>
  </html>
```
