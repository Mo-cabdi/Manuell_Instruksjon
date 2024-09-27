## Telefonkoatalogen OG DATABASER

De kan kjøres ved kopiere koden inn i terminalvinduet til MySQL/MariaDB.

Scriptene må kjøres i rekkefølgen angitt av tallene.

#### Før vi starter:

1. Logg ut av mariaDB ved å skrive
```bash
exit
```

#### Klone telefonkatalog kode og sql script fra github REPO:

2. Lag en mappe ved å skriv
```bash
mkdir Kode "Lage mappe"
```

3. Bruk CD kommando til å gå i mappe
```bash
cd Kode
```
4. Klone telefonkatalogen fra github
```bash
git clone url "eksempel: git clone https://github.com/bruker007/Kode.git"
```
---


5. Logg inn den nye brukeren.

    Også skrive inn passordret til brukeren.
```bash
mariadb -u [brukernavn] -p
```
---

9. Åpnet Kode mappen i Filutforsker og deretter åpnet alle skript filene i notisblokk.

10. Scriptene må kopieres og kjøres i rekkefølgen angitt av tallene.

##### Du har lagt din telefonkatalogen i database! Gratulerer🙌

11. Test deg og forsøk hva disse kommandoene gjør:
```bash
SELECT * FROM person;

SELECT fornavn, telefonnummer FROM person;

SELECT * FROM person WHERE fornavn = "Erik";

SELECT telefonnummer FROM person WHERE fornavn = "Lise" AND etternavn = "Pise";

INSERT INTO person (fornavn, etternavn, telefonnummer)
VALUES ('Erik', 'Perik', '12345678');

```

12. Prøve å legg en person til telefonkatalogen.






