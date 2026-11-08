# Veebiõppe märkmik

HTML-i ja CSS-i seminaritöö. Avalik repositoorium: [GeorgUT/6-praks](https://github.com/GeorgUT/6-praks).

## Avamine

Laadi repositoorium alla ja ava `index.html` brauseris. Pakettide paigaldamist ega ehitamist pole vaja.

Soovi korral käivita repositooriumi kaustas `python3 -m http.server 8000` ja ava brauseris `http://localhost:8000`.

## Failid

- `index.html` – semantiline eestikeelne veebileht.
- `style.css` – kogu kujundus eraldi failis; HTML-is pole inline-stiile.
- `images/veebikavand.svg` – selle töö jaoks loodud illustratsioon.
- `VASTUSED.md` – vastused töölehe kahele küsimusele.
- `docs/` – HTML-i ja CSS-i validaatorite tulemused.

## Töölehe ülesanded

Pealkirjal on oma värv, suurus ja Georgia font; sisutekst kasutab Arialit. Pildil on raam ja vari. Tabelil on eristuv päis ning lehel on taustavärv. Kaks sisutulpa on loodud CSS Gridiga. Kuni 760 px laiuses vaates paiknevad tulbad üksteise all.

Lähtekoodinupu liikumine kasutab ainult CSS-i `transition`- ja `transform`-omadusi. Liikumise vähendamise eelistusega kasutajale animatsiooni ei rakendata.

Kujunduse alapunktid on salvestatud eraldi commit'idesse.

## Kontrollid

Kontrollitud 8. novembril 2026:

- W3C CSS Validator, CSS3 profiil: 0 viga, 0 hoiatust.
- Nu HTML Checker: teateid ei olnud.
- Brauseris 855 × 725 px vaade: kaks tulpa, kogu sisu nähtav ilma kerimata.
- Brauseris 390 × 844 px vaade: üks tulp, horisontaalset kerimist pole.
- Nupp „Vaata lähtekoodi” avab selle repositooriumi. Repositoorium on loetav ka sisse logimata.

Validaatorite JSON-tulemused ja kontrollitud failide SHA-256 kontrollsummad on kaustas `docs/`.
