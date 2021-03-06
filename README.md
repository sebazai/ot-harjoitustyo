# Ohjelmistotekniikka - SUDOKU

Sovelluksen avulla käyttäjä pystyy pelaamaan sudoku peliä omalla tietokoneellaan. Käyttäjä pystyy tallettaa keskeneräisen pelin ja jatkamaan myöhemmin kyseistä peliä. Pelien vaikeusasteet ovat helppo, kohtalainen ja vaikea. Käyttäjä pystyy halutessaan ratkaista pelin nappia painamalla.

## Dokumentaatio

[Käyttöohje](https://github.com/sebazai/ot-harjoitustyo/blob/master/documentation/kayttoohje.md)

[Vaatimuusmäärittely](https://github.com/sebazai/ot-harjoitustyo/blob/master/documentation/vaatimusmaarittely.md)

[Arkkitehtuurikuvaus](https://github.com/sebazai/ot-harjoitustyo/blob/master/documentation/arkkitehtuuri.md)

[Testausdokumentti](https://github.com/sebazai/ot-harjoitustyo/blob/master/documentation/testaus.md)

[Tuntikirjanpito](https://github.com/sebazai/ot-harjoitustyo/blob/master/documentation/tuntikirjanpito.md)

## Releaset

### Final/Viikko 7

[Final](https://github.com/sebazai/ot-harjoitustyo/releases/tag/3.0)

### Viikko 6

[V. 2.2](https://github.com/sebazai/ot-harjoitustyo/releases/tag/2.2)

### Viikko 5

[V. 1.0](https://github.com/sebazai/ot-harjoitustyo/releases/tag/v1.0)

## Komentorivitoiminnot

### Ohjelman ajaminen
Lataa ZIP tiedosto ja pura se koneellesi. Voit aukaista projektin Netbeans:ssa tai ajaa seuraavan komennon kansiossa "sudoku":

```
mvn compile exec:java -Dexec.mainClass=sudoku.ui.SudokuUi
```

Komento

```
mvn package
```

generoi hakemistoon _target_ suoritettavan jar-tiedoston _sudoku-1.0-SNAPSHOT.jar_


### Testaus
Testit suoritetaan kansiossa sudoku, komennolla

```
mvn test
```

Kattavuusraportti testeistä luodaan komennolla

```
mvn jacoco:report
```

Kattavuusraportin voit aukaista selaimella, tiedosto sijaitsee _target/site/jacoco/index.html_

### JavaDoc

JavaDoc generoidaan komennolla

```
mvn javadoc:javadoc
```

JavaDocia voi tarkastella avaamalla selaimella tiedoston _target/site/apidocs/index.html_


### Checkstyle

Tiedoston [checkstyle.xml](https://github.com/sebazai/ot-harjoitustyo/blob/master/checkstyle.xml) määrittelemät tarkistukset suoritetaan kansiossa sudoku komennolla, komennon jälkeen tiedosto löytyy kansiosta _/sudoku/target/site/_ nimellä _checkstyle.html_

```
mvn jxr:jxr checkstyle:checkstyle
```

