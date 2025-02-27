# Talouskatsaus

Ohjelman tarkoitus on koota yhteenveto käyttäjän antamasta tiliotteesta. Ohjelma on tarkoitettu yhdelle käyttäjälle.

[Viimeisin release](https://github.com/rpessi/ot-harjoitustyo/releases/tag/viikko5)

## Python-versio

Ohjelman toiminta on testattu Python-versiolla 3.8. Erityisesti tätä vanhempien Python-versioiden kanssa saattaa
esiintyä ongelmia. 

## Dokumentaatio

- [Alustava vaatimusmäärittely](./dokumentaatio/vaatimusmaarittely.md)
- [Arkkitehtuurikuvaus](./dokumentaatio/arkkitehtuuri.md)
- [Käyttöohje](./dokumentaatio/kayttoohje.md)
- [Changelog](./dokumentaatio/changelog.md)
- [Työajan seuranta](./dokumentaatio/tuntikirjanpito.md)

## Ohjelman asennus

1. Asenna riippuvuudet komennolla:

```bash
poetry install
```

2. Käynnistä sovellus komennolla:

```bash
poetry run invoke start
```

## Komentorivitoiminnot

### Ohjelman käynnistäminen

Ohjelman pystyy käynnistämään komennolla:

```bash
poetry run invoke start
```

### Ohjelman automaattinen testaus

Automaattiset testit suoritetaan komennolla:

```bash
poetry run invoke test
```

### Testikattavuus

Testikattavuusraportin voi generoida komennolla:

```bash
poetry run invoke coverage-report
```

Raportti generoituu _htmlcov_-hakemistoon

### Pylint

Koodin laaduntarkkailijana ja tyylipoliisina toimii Pylint. Tiedoston [.pylintrc](./.pylintrc) määrittelemät 
tarkistukset voi suorittaa komennolla:

```bash
poetry run invoke lint
```
