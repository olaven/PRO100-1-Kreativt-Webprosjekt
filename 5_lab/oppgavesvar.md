# Skriftlige spørsmål fra øving

1. Hvilken velger/pseudoklasse benytter man for å angi at en CSS-endring skal skje når noe pekes på?
  * _identifikator_:hover
2. Hvilke fire parametere har transition-egenskapen?
  * transition har  
    1. property -> hvilken egenskap på elemtet skal animeres?
    2. duration -> hvor lenge skal overgange vare?
    3. timing-function -> bevegelsens hastighet, ease-in-out osv.
    4. transition-delay -> hvor lenge før animasjonen _starter_
3. Hva er de fire parameterne i transition for?
  * forrige spm.
4. Hvordan kan man angi forskjellige transition-endringer for forskjellige egenkaper på et element?
  * ved å separere med komma, f.eks.

  ``` css
    #element{
      transition: color 10s ease-in-out 0s, /*<--*/
      height 4s ease-in 1s;
  ´´´

  5. Hvordan fungerer egenskapene min-width og max-width?
    * min-width og max-width: setter henholdsvis en øvre grense for et element sin høyde og bredde.
    * overskriver av nødvendige årsaker height og width
