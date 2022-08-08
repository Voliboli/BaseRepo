# voliboli

Aplikacija, ki agregira in sprocesira statistične podatke dvoranske odbojke v Sloveniji.
Omogoča prikaz le teh in medsebojno primerjavo statistike igralcev.

## Primeri uporabe
- skupni seštevek in procentualna uspešnost igralca do tega trenutka sezone (napad,servis,sprejem) + št. odigranih tekem
- Prikaz plus/minus kako koristen je igralec ekipi skozi sezono
- Prikaz točkovne uspešnosti + napak igralca skozi sezono
- Primerjava igralcev po statistiki (side by side comparison)

## Mikrostoritve
- Uporabniki
- Igralci

### Uporabniki

    /uporabniki
    GET - vrne vse uporabnike
    POST - doda novega uporabnika
      /<uporabnik_id>
      GET - vrne podatke uporabnika
      PUT - spremeni podatke uporabnika
      DELETE - izbriše uporabnika

### Igralci

    /igralci
    GET - vrne vse igralce
    POST - doda novega igralca
      /<igralec_id>
      GET - vrne podatke igralca
      PUT - spremeni podatke igralca
      DELETE - izbriše igralca

### Uporabniška logika

Na aplikacijo se oseba najprej prijavi, potem pa jo aplikacija popelje na glavno stran, 
kjer lahko igralce dodaja, na njih pritiska za bolj podrobno statistiko/grafe ter nasplošno primerja.


## Možne nadgradnje

Kot nadgradnjo aplikacije se ahko doda primerjavo ekip po:
- win/loss razmerje
- št. blokov/asov
- uspešnost v napadu/sprejemu (perfekten sprejem v oklepaju) 
- kill-on-reception
- attack-after-dig 
- plus/minus uspesnost
- konsistentnost skozi nize
