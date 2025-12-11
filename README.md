# Balance Process Simulator
Simulatsiooniprojekt bilansihalduse ja bilansihälvete mõistmiseks.
See projekt simuleerib bilansihalduse loogikat kasutades tegelikke tarbimis-, tootmis- ja bilansihinna andmeid.  
Projekti eesmärk on näidata:
- kuidas tekivad **bilansihälbed**,  
- kuidas hälbed mõjutavad **bilansikulusid**,   
- ja kuidas neid andmeid saab visualiseerida ning analüüsida.

---
## Kasutatud tehnoloogiad
- **Python 3.11**
- **Pandas** – andmetöötlus
- **Matplotlib** – visualiseerimine
- **Jupyter Notebook** – analüüsi töövoog

---
## Analüüsiprotsessi ülevaade
### 1) Andmete allalaadimine
- Impordin tarbimise, tootmise ja prognoositud tarbimise/tootmise.
- Normaliseerin ajavormingu ja ühikud.

### 2) Prognoosi sidumine tegeliku tarbimise/tootmisega
- Tegeliku tarbimise ja tootmise prognooside ühendamine.

### 3) Bilansihälvete ja kulude arvutamine
- Arvutamine:
  - tarbimise hälve,
  - tootmise hälve,
  - netobilansihälve,
  - hälbekulud (bilansihindagega)

### Visualiseerimine
- Tarbimine vs prognoos ajas.
- Bilansihind vs netohälve.
- Päevased bilansikulud.
- Hälbekulu jaotus.

---
## Näidised

### Netohälve ja bilansihind

<img width="1189" height="490" alt="d29dc903-6cba-4f60-9e55-42573985cf74" src="https://github.com/user-attachments/assets/94bc0b08-66c3-40fb-9896-ba49936cabc2" />

- näitab millal on energiapuudus/ülejääk

### Hälve ja bilansihind 

<img width="1189" height="495" alt="732a1fea-e81e-4d5e-8172-8e2e8bd1f42d" src="https://github.com/user-attachments/assets/c80d66e1-cd64-4810-8363-cd7d333b1ff8" />

- näitab millistel perioodidel langeb halve kokku kõrge bilansihinnaga

### Netohälve ja bilansihinna korrelatsioon

<img width="790" height="490" alt="a9f480fb-3416-4a7b-8641-402e9c598712" src="https://github.com/user-attachments/assets/3d7b6fad-12cb-4dee-82f4-b99d1de75ffb" />

- näitab kas hälve kaldub tekkima kindlate bilansihinna tasemete juures

  ---
 ## Projekti käivitamine

### Terminalis:
```bash
python -m venv .venv
source .venv/bin/activate   # (Windows: .venv\Scripts\activate)
pip install -r requirements.txt
```

### Avage Jupyter:

```bash
jupyter notebook
```

### Avage notebookid järgmises järjekorras:

01_download_data.ipynb

02_generate_forecast.ipynb

03_calculate_imbalance.ipynb

04_visualizations.ipynb

