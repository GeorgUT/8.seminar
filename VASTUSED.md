# Vastused töölehe küsimustele

1. Milliseid erinevaid viise leiad, et lehe sisu jagada kahte tulpa?

Kahe tulba tegemiseks saab kasutada CSS Gridi või Flexboxi. Gridi puhul määratakse konteinerile display: grid ja grid-template-columns: 1fr 1fr. Flexboxi puhul saab konteinerile panna display: flex ning mõlemale sisuelemendile flex: 1. Kui eesmärk on jagada üks pikem tekst kahe veeru vahel, sobib column-count: 2. Võimalik on kasutada ka float'i või inline-block'i, kuid Gridi ja Flexboxiga on paigutust lihtsam hallata. Sellel veebilehel on kasutatud Gridi.

2. Miks peetakse mahukama veebilehe puhul inline-stiili halvaks tavaks?

Inline-stiil kirjutatakse otse HTML-elemendi style-atribuuti. Suurel lehel tuleb siis samu stiile paljudes kohtades korrata ja kujunduse muutmiseks peab parandama mitut elementi eraldi. See teeb koodi raskemini loetavaks ning suurendab vigade võimalust. Inline-stiilide kõrge prioriteet teeb ka nende ülekirjutamise keerulisemaks. Eraldi CSS-failiga saab samu reegleid kasutada mitmel lehel ja muuta kogu kujundust ühest kohast.
