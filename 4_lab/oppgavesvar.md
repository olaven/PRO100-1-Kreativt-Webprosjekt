# Oppgavesvar til oppgaver, lab 4

1. Hvilke verdier kan man sette på egenskapen position?
  * static
    * er default
    * alltid posijsonert etter "vanlig flow" -> måten ting legger seg på (block, inline) i html/css.
    * top, bottom, left og right fungerer _ikke_ for å posisjonere disse.
  * relative
    * blir posisjonert ut i fra den posijsonen det ville hatt derso mdet var static, men kan altså manipuleres av top, bottom, left og right.
    * dersom man flytter det, vil ikke andre elementer ta dets originale ("static") plass, men det vil stå igjen et hulrom
  * absolute
    * posijsonert i forholdt til første "parent" -> f.eks en container
  * fixed
    * posisjoneres i forlhold til viewport
    * holder seg på samme punkt uansett hvor man scroller fordi "viewport er viewport"
2. Hvordan fungerer de alternative position-egenskapene?
  * svar på oppg. 1
3. Hva gjør z-index?
  * bestemmer hvilket "lag" i dybden som elementet skal ligge på. De elementene som ligger øverst, har størst tall.
4. Det er fire egenskaper som man kan bruke for å bestemme nøyaktig plassering av et posisjonert element.
Hvilke fire er disse?
  * top, bottom, left, right 
