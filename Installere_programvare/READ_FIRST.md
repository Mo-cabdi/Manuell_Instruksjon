## Installere Programvare

* **NB:** Hopp over til neste steg om du har installert alle.

* Trykk **CTrl + Alt + T** til å åpen terminal og kjør de kommandoende.


#### Sett opp brannmur med UFW (uncomplicated Firewall)

* Installere UFW 
```bash
sudo apt install ufw    "Installere UFW"
sudo ufw enable         "Aktivere brannmur"
sudo ufw allow ssh      "tillater SSH-tilkoblinger"
sudo ufw status         "Sjekke statusen til brannmur" 
```


#### Installere SSH og skru den på

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


#### Installere MariaDB

```bash
sudo apt install mariadb-server   "Installere MariaDB"
sudo systemctl enable ssh         "Aktivere SSH"
sudo systemctl start ssh          "starter SSH"
```