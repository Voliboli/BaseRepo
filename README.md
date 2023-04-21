# voliboli

Aplikacija, ki agregira in sprocesira statistične podatke dvoranske odbojke v Sloveniji.
Omogoča prikaz le teh in medsebojno primerjavo statistike igralcev.

## Arhitektura

![Voliboli-arch (2)](https://user-images.githubusercontent.com/48418580/233632814-4b6c36d6-aa22-4492-8d75-b47bae6442dd.png)


## Primeri uporabe
- Vsak statističen podatek na tekmo posameznega igralca skozi celotno sezono
- Povprečno število točk na odigrano tekmo posameznega igralca
- Procentualno povprečje Pozitivnega sprejema, Idealnega sprejema in napada
- Število napak igralca na tekmo skozi celotno sezono (servis/sprejem/napad napake) 
- Side by side comparison igralcev + kdo je boljši

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

- vrni igralca ali samo katerokoli njegovo specifično karakteristiko
- spremeni igralcu katerokoli njegovo specifično karakteristiko
- izbriši igralca ali samo katerokoli njegovo specifično karakteristiko

### Uporabniška logika

Na aplikacijo se oseba najprej prijavi, potem pa jo aplikacija popelje na glavno stran, 
kjer lahko igralce ali ekipe dodaja, na njih pritiska za bolj podrobno statistiko/grafe ter nasplošno primerja.


## Možne nadgradnje

Kot nadgradnjo aplikacije se lahko doda primerjavo ekip po:
- kill-on-reception
- attack-after-dig 
- konsistentnost skozi nize
- Primerjava igralcev po karakteristikah (višina, teža, sprejemalci, podajači)
