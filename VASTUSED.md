# Vastused töölehe küsimustele

Veebilehe avalik GitHubi repositoorium: https://github.com/GeorgUT/6-praks

1. Milliseid erinevaid viise leiad, et lehe sisu jagada kahte tulpa?

Sisu saab jagada kaheks tulbaks mitmel viisil:
- CSS Grid: konteinerile määratakse display: grid ja grid-template-columns: 1fr 1fr. Nii tekib kaks võrdse laiusega tulpa. Seda lahendust kasutasin oma veebilehel.
- Flexbox: konteinerile määratakse display: flex ning mõlemale sisuelemendile flex: 1. Elementide vahele saab lisada gap-iga vahe.
- CSS-i mitmeveeruline paigutus: column-count: 2 jaotab ühe järjestikuse teksti kahe veeru vahel. See sobib näiteks artiklile, mille tekst peab voolama ühest veerust teise.
- Vanemad võimalused on float ja display: inline-block koos sobivate laiustega. Tänapäeval on iseseisvate sisutulpade jaoks üldjuhul mugavamad Grid ja Flexbox.

Väikesel ekraanil saab media query abil kaks tulpa üheks muuta, et sisu jääks loetavaks.

2. Miks peetakse mahukama veebilehe puhul otse HTML-elementide küljes olevat stiili (inline style) halvaks tavaks?

Inline-stiil segab lehe sisu ja kujunduse ning muudab HTML-i mahukamaks ja raskemini loetavaks. Sama kujundust tuleb sageli mitme elemendi juures korrata, mistõttu nõuab üks muudatus paljude kohtade parandamist ning kujundus võib muutuda ebaühtlaseks. Inline-stiilidel on tavaliste stiilifaili reeglite ees kõrge prioriteet, mis teeb nende ülekirjutamise keerulisemaks. Samuti ei saa style-atribuudis otse määratleda @media reegleid ega :hover- ja :focus-olekuid. Eraldi CSS-fail võimaldab kujundusreegleid taaskasutada mitmel lehel, neid ühest kohast muuta ning brauseril stiilifaili vahemällu salvestada.
