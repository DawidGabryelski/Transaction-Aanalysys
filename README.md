# Kajo Data Space - Analiza sprzedaży

## Cele projektu i opis
Projekt koncentruje się na zaawansowanej analizie danych transakcyjnych w celu zrozumienia retencji klientów (Customer Retention). Wykorzystując technikę analizy kohortowej, zbadano zachowanie grup użytkowników pozyskanych w konkretnym czasie na przestrzeni kolejnych miesięcy ich cyklu życia w usłudze.

## Stack Techniczny
* **Analiza danych:** Pandas
* **Środowisko:** Jupyter Notebook / VS Code
* **Wizualizacja:** Power BI (DAX)

## Struktura Danych i Przetwarzanie
Analiza opiera się na rzeczywistym zbiorze transakcji, który został poddany procesom czyszczenia i transformacji. Główne elementy analizy obejmują:
* Analizę kohortową (Cohort Analysis).
* Badanie lojalności klientów (Retention Rate).
* Analizę dynamiki przychodów YoY (Year-over-Year).
* Segmentację klientów według wartości wpłat.

## Retencja w ujęciu kohortowym
Ta sekcja raportu skupia się na analizie grup użytkowników, którzy dołączyli do usługi w określonych przedziałach czasowych.

### Filtr
Przedstawia kohorty w formacie rok-miesiąc. Jest to kluczowy element nawigacyjny pozwalający na izolację konkretnych grup i śledzenie ich aktywności w czasie.

### Wykres liniowy
Wizualizacja prezentuje liczbę nowych, unikalnych klientów. Przy braku aktywnych filtrów widoczna jest linia trendu ogólnego. Po wybraniu konkretnej kohorty, wykres wyświetla drugą linię obrazującą sytuację danej grupy na tle całej populacji. Zastosowano tutaj miarę DAX z funkcją REMOVEFILTERS, co pozwala na porównanie danych przefiltrowanych z nieprzefiltrowaną bazą.

### Wykres lejkowy
Dodany w celu wyeliminowania trudności w interpretacji zmian przy niskich wartościach na wykresie liniowym. Pozwala na precyzyjną ocenę spadków liczebności grupy w kolejnych etapach.

### Zakładki Podsumowanie i rekomendacje
System zakładek pozwala na szybkie przełączanie się między automatycznym podsumowaniem danych a wnioskami biznesowymi.

#### Podsumowanie
Pole tekstowe generujące dynamiczny opis dostosowany do wybranego filtra. Zawiera informacje o wielkości grupy początkowej, wygenerowanym przychodzie oraz liczbie klientów pozostających w usłudze do dnia 31.03.2026.

#### Rekomendacje
Zawierają konkretne propozycje działań naprawczych i optymalizacyjnych:
* **Przeciwdziałanie rezygnacji:** Ze względu na wysoki wskaźnik churn po pierwszym miesiącu, sugerowane jest wprowadzenie planów 3-miesięcznych z atrakcyjnym systemem rabatowym.
* **Aktywacja powracających:** Rekomendowane jest oferowanie zniżek motywacyjnych w zamian za wypełnienie formularza zwrotnego, co pozwoli na zebranie danych o przyczynach rezygnacji.

### Dokumentacja wizualna - Retencja
| Bez aktywnego filtra | Aktywny filtr | Zakładka rekomendacje |
| :--- | :--- | :--- |
| <img width="958" alt="Strona 1-1" src="https://github.com/user-attachments/assets/39f7121f-8936-4435-8dfd-12a612be43d2" /> | <img width="962" alt="Strona 1-2" src="https://github.com/user-attachments/assets/8009e3ca-86e7-4a79-bada-3a18d7f2e366" /> | <img width="957" alt="Strona 1-3" src="https://github.com/user-attachments/assets/1cf9ee2b-31e7-4d17-8ff7-74684cb681d4" /> |

## Przegląd ogólny klientów
Sekcja dedykowana całościowej analizie sprzedaży w Kajo Data Space.

### Tabela zbiorcza
Prezentuje łączny przychód oraz liczbę nowych klientów w ujęciu rocznym i kwartalnym, wraz ze wskaźnikiem wzrostu procentowego rok do roku (YoY%).

### Wykres kolumnowy
Przedstawia segmentację klientów na podstawie wpłaconych kwot (przedziały co 500 PLN). Etykiety wskazują liczebność użytkowników w każdym segmencie.

### Wnioski biznesowe
* **Dynamika rozwoju:** Stały wzrost przychodów potwierdza skuteczność działań marketingowych i wysoką jakość oferowanych usług.
* **Struktura bazy:** Główny udział w przychodach mają nowi klienci o krótkim cyklu życia w usłudze. Priorytetem strategicznym powinno być wdrożenie mechanizmów retencyjnych w celu stabilizacji bazy stałych użytkowników.

### Dokumentacja wizualna - Przegląd ogólny
| Podsumowanie ogólne | Rekomendacje ogólne |
| :--- | :--- |
| <img width="956" alt="Strona 2-1" src="https://github.com/user-attachments/assets/1cf9ee2b-31e7-4d17-8ff7-74684cb681d4" /> | <img width="962" alt="Strona 2-2" src="https://github.com/user-attachments/assets/b3626f6e-3250-42a4-b49e-4ba69db7a937" /> |

---
**Autor:** [Dawid Gabryelski](https://github.com/DawidGabryelski)
