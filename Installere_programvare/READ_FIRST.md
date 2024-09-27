## Installere Programvare

* **NB:** Hopp over til neste steg om du har installert alle.

* Trykk **CTrl + Alt + T** til å åpen terminal og kjør de kommandoende.


#### Sett opp brannmur med UFW (uncomplicated Firewall)

Brannmuren tillater andre maskiner å snakke med programmer på serveren ved å åpne porten
("husnummeret") som programmet kjører på. Her åpner vi port 22, som er den porten SSH kommuniserer på.


* Installere UFW 
```bash
sudo apt install ufw    "Installere UFW"
sudo ufw enable         "Aktivere brannmur"
sudo ufw allow ssh      "tillater SSH-tilkoblinger"
sudo ufw status         "Sjekke statusen til brannmur" 
```


#### Installere SSH og skru den på


SSH er et program som lar oss logge på en datamaskin fra en annen datamaskin via nettverket. Vi har
installert det i steget over, men må også starte det, og sørge for at det starter automatisk hver gang vi skrur
på serveren.

```bash
sudo apt install openssh-server   "Installere SSH"
sudo systemctl enable ssh         "Aktivere SSH"
sudo systemctl start ssh          "starter SSH"
```
**NB** 
```bash
ip a   "Finn IPen din. Du trenger til å bruker SSH"
```
* Hvis du har kablet nettverk, vil IP vises ved eth0: linje. Hvis du kun har trådløst, vil ip vises ved wlan0: linje. IP-adresse er vanligvis 10.2.3.x eller noe lignende (hvor x er et nummer mellom 2 og 254)

---


#### Installere MariaDB, python og git

```bash
sudo apt install python3-pip         
sudo apt install git
sudo apt install mariadb-server
sudo mysql_secure_installation     
```

Good jobb, da er du klar til [neste_steg](/Sette_opp_Database/READ_FIRST.md).

Good jobb, da er du klar til [neste_steg](/Sette_opp_Database/READ_FIRST.md).