# Absenteeism at Work — Analiza danych

Projekt zawiera analizę danych dotyczących absencji w pracy. Celem jest eksploracja danych, przygotowanie cech i zbudowanie prostego modelu przewidującego brak obecność/przyczyny absencji oraz demonstracja typowego pipeline'u ML.

## Zawartość repozytorium
- `Absenteeism_at_Work.ipynb` — główny notebook z analizą i modelowaniem.
- `Data/Absenteeism_at_work.csv` — dane w formacie CSV.
- `Data/Absenteeism_at_work.arff` — dane w formacie ARFF (orig.).

## Dane
Zestaw danych zawiera informacje o pracownikach i ich nieobecnościach (godziny nieobecności, przyczyny, wiek, czas pracy itp.).

## Wymagania
Zalecane jest użycie wirtualnego środowiska Python (venv/conda). Przykładowe pakiety wymagane do uruchomienia notebooka:

```
python -m venv .venv
source .venv/Scripts/activate   # Windows: .venv\Scripts\activate
pip install --upgrade pip
Można użyć pliku `requirements.txt` z listą zależności (załączony w repozytorium). Aby zainstalować pakiety z pliku:

```bash
pip install -r requirements.txt
```

Aby wygenerować `requirements.txt` z aktualnego (aktywnego) środowiska:

```bash
pip freeze > requirements.txt
```
```

## Uruchomienie
1. Aktywuj środowisko wirtualne.
2. Uruchom Jupyter/ JupyterLab w katalogu projektu:

```bash
jupyter notebook Absenteeism_at_Work.ipynb
```

3. Przeglądaj komórki notebooka krok po kroku: najpierw sekcja EDA (eksploracyjna analiza danych), potem preprocess, trenowanie modeli i ewaluacja.

## Workflow w notebooku
- Wczytanie danych i szybki podgląd (head, info, describe)
- Czyszczenie i obsługa brakujących wartości
- Inżynieria cech i skalowanie
- Podział na zbiór treningowy/testowy
- Trenowanie i porównanie prostych modeli (np. Logistic Regression, RandomForest)
- Ewaluacja (accuracy, precision, recall, confusion matrix)
- Wizualizacje istotnych zależności

## Źródła
Dane w folderze `Data/` pochodzą z pliku `Absenteeism_at_work.arff`.

