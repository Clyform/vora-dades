# Dades obertes d'activitats dels equipaments públics de Barcelona

Recull automàtic i normalitzat de l'oferta d'activitats dels centres cívics,
casals de barri, biblioteques i museus de Barcelona.

Aquest repositori **només conté dades**. Es regenera cada nit de manera
automàtica i no s'hi treballa a mà.

## Fitxers

| Fitxer | Què és |
|---|---|
| `data/activities.json` | Activitats amb dates, horaris, preu, estat d'inscripció i equipament |
| `data/venues.json` | Equipaments amb adreça, contacte i coordenades |
| `data/meta.json` | Data de generació, recomptes, barris i categories |

`meta.json` és petit (~30 KB) i porta `generatedAt`: serveix per saber si hi ha
res nou sense haver de descarregar la resta.

## Procedència i llicència

**Agenda d'activitats i esdeveniments de la ciutat de Barcelona** — Open Data
BCN, Ajuntament de Barcelona. Dataset
[`agenda-diaria`](https://opendata-ajuntament.barcelona.cat/data/ca/dataset/agenda-diaria),
llicència **[Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/deed.ca)**.

La part que en prové conserva la mateixa llicència. Si la fas servir, mantén
l'atribució a l'**Ajuntament de Barcelona**.

**Catàleg de cursos dels centres cívics** — informació factual (títols, dies,
horaris, preus) publicada pels propis equipaments als seus webs. Els fets no
són objecte de copyright.

Les imatges **no** es guarden aquí: les fitxes apunten als servidors dels
titulars corresponents.

## Advertiments

- Les dades provenen de tercers i **poden ser incorrectes o desactualitzades**.
  La font oficial sempre és el web del centre corresponent.
- Quan un equipament deixa de respondre, es conserva la seva última informació
  bona i es marca amb `stale: true`. Comprova aquest camp abans de fiar-te'n.
- Sense cap relació amb l'Ajuntament de Barcelona ni amb els equipaments que hi
  surten. Projecte independent.

## Persones que hi surten

El catàleg inclou noms de talleristes, tal com els publiquen els propis centres
als seus webs, en context professional i sense dades de contacte personals. Si
sou una d'aquestes persones i voleu que el vostre nom no hi consti, obriu una
*issue* i s'esborrarà a la següent regeneració.
