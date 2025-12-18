# Flask-prosjekt – Dokumentasjon

## 1. Forside

**Prosjekttittel:**  
WebNovelHub  

**Navn: Supreme*\
**Klasse:** 2IMI  
**Dato:** 27.11.2025  

**Kort beskrivelse av prosjektet:**  
Dette prosjektet er en enkel nettside hvor brukeren kan lage webromaner og skrive kapitler. Romaner og kapitler lagres i en MariaDB-database, og vises på nettsiden gjennom Flask.

---

## 2. Systembeskrivelse

**Formål med applikasjonen:**  
Å lage en liten webplattform der du kan lese webnoveller og lage egne kapitler.

**Brukerflyt (kort):**  
- Brukeren åpner nettsiden  
- Klikker på “Novels” for å se alle romaner  
- Brukeren kan lage en ny roman  
- Inne i en roman kan brukeren lage kapitler  
- Kapitlene vises i rekkefølge og kan leses eller slettes  

**Teknologier brukt:**  
- Python / Flask  
- MariaDB  
- HTML / CSS  
- Raspberry Pi som server  

---

## 3. Server-, infrastruktur- og nettverksoppsett

### Servermiljø  
- Raspberry Pi som kjører Flask  
- MariaDB som database  

### Nettverksoppsett  
- Raspberry Pi på lokalt nettverk  
- Flask kjører på port 5000  

---

## 4. Prosjektstyring – GitHub Projects (Kanban)

Kanban-board brukt med:  
- To Do  
- In Progress  
- Done  


---

## 5. Databasebeskrivelse

**Databasenavn:**  
webnovels

## 6. Programstruktur

```
project/
 ├── app.py
 ├── templates/
 ├── static/
 └── README.md
```

Databasestrøm:

```
HTML → Flask → MariaDB → Flask → HTML
```

---

## 7. Kodeforklaring (kort)

Flask-ruter:  
- `/novels` – viser alle romaner  
- `/novel/<id>` – viser info og kapitler til en roman  
- `/novel/new` – lage ny roman  
- `/novel/<id>/chapter/new` – lage nytt kapittel  
- `/chapter/<id>` – lese et kapittel  

---

## 8. Sikkerhet og pålitelighet

- Parameters


---

## 9. Feilsøking og testing

- SQL-feil førte til internal server error  
- Manglende ruter ga 404  
- Glemte å skru på rasberry pi

**Testing:**  
- Testet creation og sletting av romaner  
- Testet kapitler  
- Testet navigasjon

---

## 10. Konklusjon og refleksjon

Jeg lærte å sette opp Flask med MariaDB og lage et fungerende websystem.  
Jeg ville lagt til innlogging og brukere hvis jeg visste litt mer

---

## 11. Kilder

- w3schools  
