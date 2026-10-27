<div align="center">

# Absenteeism at Work

**Analiza absencji pracowników — od eksploracji danych po przygotowanie i ewaluację modeli uczenia maszynowego.**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-data%20analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![scikit--learn](https://img.shields.io/badge/scikit--learn-machine%20learning-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

</div>

---

## O projekcie

Projekt zawiera analizę danych dotyczących absencji w pracy. Notebook prowadzi przez eksplorację danych, przygotowanie cech oraz trenowanie i ocenę przykładowych modeli przewidujących nieobecności.

## Zawartość repozytorium

| Plik | Opis |
| --- | --- |
| `Absenteeism_at_Work.ipynb` | Główny notebook z analizą danych i modelowaniem |
| `Data/Absenteeism_at_work.csv` | Dane źródłowe w formacie CSV |
| `Data/Absenteeism_at_work.arff` | Dane źródłowe w formacie ARFF |
| `requirements.txt` | Lista pakietów Python wymaganych do pracy z projektem |

## Analiza obejmuje

- Wczytanie danych i przegląd ich struktury oraz statystyk
- Czyszczenie danych i obsługę brakujących wartości
- Inżynierię cech i skalowanie
- Podział danych na zbiory treningowy i testowy
- Trenowanie i porównanie modeli, np. regresji logistycznej i Random Forest
- Ewaluację modeli za pomocą accuracy, precision, recall i macierzy pomyłek
- Wizualizację zależności w danych

## Technologie

- **Język:** Python
- **Analiza danych:** pandas, NumPy
- **Uczenie maszynowe:** scikit-learn
- **Wizualizacje:** Matplotlib, Seaborn
- **Notebooki:** JupyterLab
- **Format danych:** CSV, ARFF (`liac-arff`)

## Wymagania

- Python 3
- Pakiety wymienione w `requirements.txt`

## Uruchomienie

### 1. Przygotuj środowisko

W katalogu projektu utwórz i aktywuj wirtualne środowisko:

```bash
python -m venv .venv
```

Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

macOS / Linux:

```bash
source .venv/bin/activate
```

### 2. Zainstaluj zależności

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 3. Uruchom notebook

```bash
jupyter notebook Absenteeism_at_Work.ipynb
```

Możesz też uruchomić JupyterLab poleceniem `jupyter lab`. W notebooku wykonuj komórki po kolei — od eksploracyjnej analizy danych (EDA), przez preprocessing i trenowanie modeli, po ewaluację.

## Źródła danych

Dane znajdujące się w folderze `Data/` pochodzą ze zbioru `Absenteeism_at_work.arff`.
