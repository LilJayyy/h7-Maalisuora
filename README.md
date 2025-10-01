# h7-Maalisuora

## Sisältö

[a) Hei Maailma](#a-Hei-Maailma)

[b) Lähdeviitteet](#b-Lähdeviitteet)

[c) Komento](#c-Komento)

[d) Laboratorioharjoitus](#d-Laboratorioharjoitus)


### Koneen tekniset tiedot
* Prosessori: Intel Core i5-8265U CPU @ 1.60 GHz (1.80 GHz turbo, 8 ydintä)
* RAM: 16 GB (15,7 GB käytettävissä)
* Järjestelmä: Windows 11 Pro 64-bittinen (x64-suoritin)
* Näytönohjain: Intel UHD Graphics 620
* Tallennustila: 237 GB, josta 158 GB vapaana
* DirectX-versio: DirectX 12



# a) Hei Maailma

Lähdin tässä tehtävänosiossa 1.10.2025 kello 18:40 etenemään seuraavasti. Tarkoitus oli siis kirjoittaa ja ajaa kolmella kielellä. 

Tässä käytin Karvisen (2018) ohjeistusta ja tunnilla samaan aikaan opittua.

Valitsin hänen ohjeestaan Pythonin, Bashin ja Luan.

## Python

Tähän kieleen olikin jo aikaisemmin kerennyt tutustua. Se oli asennettuna jo valmiiksi, joten jätän asennusvaiheen tässä osiossa pois.

Loin tiedoston
* **`nano hello.py`** 

Kirjoitin sisällön
* **`print ("Hei maailma")`**
  - Ctrl + O
  - Ctrl + X

Ajoin sen
* **`python3 hello.py`** 

![2](images/2.png)

_Nanoon haluttu sisältö_

![1](images/1.png)

_Nätisti tulostui_

## Bash

Tätä kerkesin jo kokeilla tunnin aikana Johannan opastuksella.

1. Tiedoston luominen
* **`nano hello.sh`** 

2. Sisältö koodeineen sinne
* **`#!/bin/bash 
echo "Hei maailma"`**
  - Ctrl + O
  - Ctrl + X

3. Annoin oikeudet ajamiseen
* **`chmod +x hello.sh`** 

4. Ajoin sisällön
* **`./hello.sh`** 

![4](images/4.png)

_Komennot prosessissa_

## Lua

1. Asensin sen ensin alla olevalla komennolla:
* **`sudo apt-get install lua5.4`**
  - syötin salasanan ja Enter
  
![6](images/6.png)

_Lua asennusta_

2. Loin tiedoston 
* **`nano hello.lua`**

![5](images/5.png)

_Nanon sisältö_

3. Sisältö sinne
* **`print("Hei maailma")`**
  - Ctrl + O
  - Ctrl + X

4. Ajoin sisällön
* **`print("Hei maailma")`** 

![7](images/7.png)

_Lua:lla tulostusta_



# b) Lähdeviitteet

* Tämä tehtävänosio oli jo tehty tätä raporttia kirjoittaessa, sillä vittasin kaikkin lähteisiin ohjeistusten mukaisesti niitä tehdessä. 

# c) Komento

Tähän tehäväosioon siirryin samana päivänä 1.10.2025 kello 19:22.

### Skripti

Tätäkin tehtävänosaa seurasin tunnin aikana, jota oli helppo tehdä tässä samalla.

1. Loin tiedoston `Tervetuloa` nanolla komennolla:
* **`nano Tervetuloa`**

2. Sisältöä skriptiin
* **`#!/bin/bash`
echo "Tervetuloa Linuxiin!"`**
  - Ctrl + O
  - Ctrl + X

3. Annoin oikeudet ajamiseen
* **`chmod +x Tervetuloa`**

4. Kopioin käyttäjille skriptin pääkäyttäjän roolissa
* **`sudo cp Tervetuloa /usr/local/bin/`**

5. Ajetaan ja testausta
* **`Tervetuloa`**

![9](images/9.png)

_Yllä oleva prosessi kuvina eli tehty komentoni_
  
# Vanha laboratorioharjoitus

[d) howdy](#d-howdy)

[e) Etusivu uusiksi](#e-Etusivu-uusiksi)

[g) Salattua hallintaa](#g-Salattua-hallintaa)

[h) Djangon lahjat](#h-Djangon-lahjat)

Saman päivänä 1.10.2025 siirryin kello 19:57 tämän osion pariin. 

Valitsin _Final Lab for Linux Palvelimet 2024 Spring_ eli viime vuoden kevään laboratorioharjoituksen ja sovelsin sitä ohjeistuksen mukaan tarvittaessa.

## d) 'howdy'

`Tehtävänantona oli:
- Tee kaikkien käyttäjien käyttöön komento 'howdy'
- Tulosta haluamaasi ajankohtaista tietoa, esim päivämäärä, koneen osoite tms
- Pelkkä "hei maailma" ei riitä
- Komennon tulee toimia kaikilla käyttäjillä työhakemistosta riippumatta`

Tästä tein ylempää juuri vastaavan, joten tämä osuus oli vielä erittäin hyvin muistissa.

1. Päivitin ensin paketit välissä
* **`sudo apt-get update`**

2. Nanolla tiedosto 
* **`nano howdy`**

3. Annoin oikeudet ajoon
* **`chmod +x howdy`**

4. Kopioin käyttäjille skriptin pääkäyttäjän roolissa
* **`sudo cp howdy /usr/local/bin/`**

5. Testaus
* **`howdy`**

![9](images/9.png)

_Onnistunut komennolla tulostus_



## e) Etusivu uusiksi

Tässä tehtäväosiossa hyödynsin omaa raporttiani h3 Maailma kuulee ja Karvisen (2018) ohjetta.

Tämäkin vaihe meni kyllä todella hyvin ulkomuistista suurimmalta osin.

1. Pakettien päivitystä
* **`sudo apt-get update`**

Apache on jo asennettu, joten sitä prosessia en tässä kohtaa raporttia käy läpi.


2. Loin uuden kansion kotihakemistoon ja kirjoitin web-sivun sisällön index.html tiedostoon nanolla
* **`mkdir -p ~/public_html`**
* **`nano ~/public_html/index.html`**

Sisältö on alla oleva sillä halusimme tehtävänosiossa kotisivn "Al Kakone":

```
<!DOCTYPE html>
<html>
<head>
    <title>AI Kakone</title>
</head>
<body>
    <h1>Tervetuloa AI Kakoneen kotisivulle!</h1>
</body>
</html>
```


* **`hostname -I`** komennolla muistelin virtuaalikoneen IP-osoitetta joka oli `10.0.2.15`.

Tässä kohtaa ilmeni virhetilanne:
Se vei minut väärälle sivulle eli oletushakemiston HTML-sisältöön, eikä juuri luomaani käyttäjän liljas sisältöön.

Olin kirjoittanut virtuaalikoneen internet-selaimen hakukenttään `10.0.2.15` oikean `http://10.0.2.15/~liljas/` sijaan. 

Tajusin onneksi nopeasti virhetilanteen, ja pääsin hienosti alla olevaan näkymään:

![20](images/20.png)

_Uusi Al Kakone kotisivu_


## e) Salattua hallinta

- Asenna ssh-palvelin
- Tee uusi käyttäjä omalla nimelläsi, esim. minä tekisin "Tero Karvinen test", login name: "terote01"
- Automatisoi ssh-kirjautuminen julkisen avaimen menetelmällä, niin että et tarvitse salasanoja, kun kirjaudut sisään. Voit käyttää kirjautumiseen localhost-osoitetta




## h) Djangon lahjat

# Lähteet

Karvinen, T. 2025. Verkkosivu. _Linux Palvelimet 2025_ alkusyksy Luettavissa: https://terokarvinen.com/linux-palvelimet/ Luettu: 20.08.2025.

Karvinen, T. 2018. Artikkeli. Name Based Virtual Hosts on Apache – Multiple Websites to Single IP Address Luettavissa: https://terokarvinen.com/2018/04/10/name-based-virtual-hosts-on-apache-multiple-websites-to-single-ip-address/ Luettu: 05.09.2025.

Karvinen, T. 2018. Verkkosivu. _Hello World Python3, Bash, C, C++, Go, Lua, Ruby, Java – Programming Languages on Ubuntu 18.04_ Luettavissa: https://terokarvinen.com/2018/hello-python3-bash-c-c-go-lua-ruby-java-programming-languages-on-ubuntu-18-04/ Luettu: 1.10.2025.

Karvinen, T. 2024. Verkkosivu. _Final Lab for Linux Palvelimet 2024 Spring_ Luettavissa: https://terokarvinen.com/2024/arvioitava-laboratorioharjoitus-2024-linux-palvelimet/ Luettu: 1.10.2025
