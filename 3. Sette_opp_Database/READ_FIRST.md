## Databaser


* **NB:** Hopp over til neste steg hvis du gjort det før.


#### Lag ny database bruker og sett riktig rettigheter.
a.  Logg inn i MariaDB
```bash
sudo mariadb -u root
```

b.  Lag ny bruker
```bash
CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';
```

c. Gi ny bruker rettigheter
```bash
GRANT ALL PRIVILEGES ON *.* TO 'username'@’localhost’ IDENTIFIED BY 'password';
```

d. Oppdater rettigheter
```bash
FLUSH PRIVILEGES;
```


Good jobb, da er du klar til [neste_steg](/Telefonkatalog/README_FIRST.md).