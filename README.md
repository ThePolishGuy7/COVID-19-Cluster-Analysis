# COVID-19 Cluster Analysis

**[Opis w języku polskim]**

Ten projekt został stworzony jako praca zaliczeniowa w ramach przedmiotu **Eksploracyjna Analiza Danych** na studiach. Jego głównym celem było przeprowadzenie hierarchicznej analizy skupień na wczesnych danych dotyczących pandemii COVID-19 (od 11 lutego do 22 marca 2020 roku).

**Źródła danych:**
Projekt opiera się na zbiorze danych epidemicznych udostępnionym przez prowadzącą, który został połączony z zewnętrznymi danymi demograficznymi Organizacji Narodów Zjednoczonych (ONZ) pochodzącymi z 2019 roku. Dodane zmienne demograficzne to m.in. wielkość populacji, gęstość zaludnienia oraz mediana wieku w poszczególnych państwach.

*Uwaga: Główny plik z kodem (RMarkdown - `.Rmd`) oraz wygenerowany na jego podstawie raport PDF są w całości napisane w języku polskim.*

### Zawartość projektu
Analiza została przeprowadzona w języku R i obejmuje pełny proces badawczy:
* **Eksploracyjną Analizę Danych (EDA):** Kompleksowe wizualizacje, w tym animowane i interaktywne mapy przestrzenne (z wykorzystaniem m.in. pakietów `plotly` i `sf`), obrazujące rozwój pandemii w czasie.
* **Przetwarzanie i Inżynierię Cech:** Oczyszczenie danych, transformacja formatów oraz stworzenie wskaźników relatywnych, takich jak wskaźnik zachorowalności (Incidence Rate) czy śmiertelności (Mortality Rate), pozwalających na rzetelne porównanie państw.
* **Hierarchiczną Analizę Skupień:** Zbudowanie modelu przy użyciu odległości euklidesowej i metody Warda (Ward.D2), który podzielił państwa na 7 unikalnych klastrów o zróżnicowanym przebiegu epidemii.
* **Walidację K-średnich (K-Means):** Zweryfikowanie stabilności uzyskanych wyników za pomocą nienadzorowanego algorytmu podziałowego (K-średnich) oraz optymalizacji hiperparametrów metodą Grid Search.
* **Szczegółową interpretację:** Opis charakterystyki wyodrębnionych grup państw (np. zidentyfikowanie "Strefy Zero" czy klastrów państw gęsto zaludnionych, które szybko wdrożyły obostrzenia).

---

**[English Description]**

This project was created as a final assignment for the **Exploratory Data Analysis** university course. The main objective was to perform a hierarchical cluster analysis on early COVID-19 pandemic data (covering the period from February 11 to March 22, 2020).

**Data Sources:**
The project utilizes an epidemiological dataset provided by the course instructor, which was merged with external demographic data from the United Nations (UN) from 2019. The demographic data includes population size, population density, and median age for individual countries.

*Note: The main source code file (RMarkdown - `.Rmd`) and the compiled PDF report are written entirely in Polish.*

### Project Overview
The analysis was performed in R and covers the entire data science research process:
* **Exploratory Data Analysis (EDA):** Comprehensive visualizations, including animated and interactive spatial maps (using packages like `plotly` and `sf`), illustrating the global spread of the virus over time.
* **Data Preprocessing & Feature Engineering:** Data cleaning, format transformations, and the creation of relative metrics like Incidence Rate and Mortality Rate to allow objective comparison between countries of varying sizes.
* **Hierarchical Clustering:** Building a model using Euclidean distance and Ward's method (Ward.D2) to divide countries into 7 distinct clusters based on their pandemic progression profiles.
* **K-Means Validation:** Verifying the stability of the hierarchical structures using the partitioning K-Means algorithm, supported by a Grid Search hyperparameter optimization.
* **In-depth Interpretation:** Detailed profiling of the resulting clusters (e.g., identifying the pandemic's "Ground Zero" or clusters of highly populated Asian countries that managed to quickly contain the spread).