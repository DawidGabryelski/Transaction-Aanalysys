# Kajo Data Space - Analiza sprzedaży

## 1. Cele projektu i opis

Jest to projekt konkursowy który skupia się na analizie danych transakcyjnych KajoDataSpace od początku jego istnienia. Projekt zawiera dwie strony. 
Retencja w ujęciu kohortowym oraz przegląd ogólny klientów.

## 2. Retencja w ujęciu kohortowym

Ta strona składa się z pięciu elementów i skupia się an analizie grup które dołączyły w konkretnych okresach:

### a) Filtr 

Filtr przedstawia kohorty w formie rok-miesiąc które symbolizują czas w jakim pojawiali się kolejni klienci. Korzystanie z niego jest niezbędne do prawidłowej analizy kohortowej.

### b) Wykres liniowy

Gdy nie mamy zaznaczonego żadnego filtru widać tylko jedną linię która pokazuje nowych, unikalnych klientów na przestrzeni całej osi czasu. Gdy skorzystamy z filtra pojawi się drug linia
symbolizująca jak wyglądała sytuacja danej grupy na tle wszystkich klientów. Zostalo to osiągnięte za pomocą miary DAX z funkcją REMOVWFILTERS. Dzięki temu na wykresie znajdują się zarówno 
linia stała jak i dynamiczna.

### c) Wykres lejkowy

Jako że interpretacja zmian w wybranej kohorcie na wykresie liniowym może być trudna przy niskich wartościach i nie zmieniającej się osi, dodany został wykres lejkowy który pozwala na dokładną 
analizę grupy nawet przy niskich wartościach.

### d) Zakładki Podsumowanie i rekomendacje

Oddzielają one dwa pola tekstowe zawierające podsumowanie informacji na dashboardzie oraz rekomendacje dla odbiorcy.

#### d1) Podsumowanie  

Pole tekstowe które zawiera dynamiczny tekst który dostosowywuje się do wartości filtra. Możemy tam znaleźć informację o wybranej grupie, jej stanie początkowym, przychodzie wygenerowanym przezcałą tą grupę liczbie pozostałych klientów, oraz liczbie klientów będących od momentu dołączenia (wybrany filtr) do dnia dzisiejszego - 31.03.2026

#### d2) Rekomendacje 

To pole zawiera rekomendacje dla odbiorcy - jeden z wymogów konkursowych.Oto pełna treść rekomendacji:

* **Ucieczka po miesiącu:** Analiza kohortowa wskazuje, że większość nowych klientów rezygnuje już po pierwszym miesiącu.
Zaleca się wprowadzenie atrakcyjnych planów 3-miesięcznych, oferujących wyższy rabat niż plan miesięczny. Pozwoli to klientom na
dłuższą perspektywę zapoznania się z treściami, przy jednoczesnym uniknięciu bariery wysokiego kosztu planu rocznego.

*  **Co zrobić z powracającymi klientami?**:  W celu aktywacji powracających użytkowników rekomendowane jest wprowadzenie zniżek motywacyjnych.
Warunkiem otrzymania rabatu powinno być wypełnienie krótkiego formularza. Pozwoli to na zebranie cennych danych o przyczynach 
wcześniejszych rezygnacji i pomoże w optymalizacji usługi w przyszłości.

### Retencja w ujęciu kohortowym - Bez aktywnego filtra 

<img width="958" height="537" alt="Strona 1-1" src="https://github.com/user-attachments/assets/39f7121f-8936-4435-8dfd-12a612be43d2" />

### Retencja w ujęciu kohortowym - Aktywny flitr

<img width="962" height="541" alt="Strona 1-2" src="https://github.com/user-attachments/assets/8009e3ca-86e7-4a79-bada-3a18d7f2e366" />

### Retencja w ujęciu kohortowym - Zakładka rekomendacje

<img width="957" height="536" alt="Strona 1-3" src="https://github.com/user-attachments/assets/108b273d-7f6a-4413-9eeb-5e286a794677" />


## 3. Przegląd ogólny klientów 

Ta strona składa się z czterech elementów i skupia się na analizie całości sprzedaży KajoDataSpace:

### a) Tabela 

W tabeli znajdziemy łączny przychód i liczbę nowych, unikalnych klientów w ujęciu rocznym i kwartalnym oraz wzrost procentowy w stosunku do tego samego okresu rok wcześniej YoY%

### b) Wykres kolumnowy

Zawiera on przedziały z w których umieszczani są klienci którzy wpłacili określoną kwatę. Kwoty są dzielone co 500 złotych a w etykietach na górze została umieszczona liczba klientów która mieści się w danym przedziale.

### c) Zakładki Podsumowanie i rekomendacje

Oddzielają one dwa pola tekstowe zawierające podsumowanie informacji na dashboardzie oraz rekomendacje dla odbiorcy.

#### c1) Podsumowanie

Znajduje się tu informacja o medianie i pierwszym kwartylu z łącznych wpłat klientów oraz podsumowanie najważniejzych osiągnięć.

#### c2 Rekomendacje 

To pole zawiera rekomendacje dla odbiorcy - jeden z wymogów konkursowych.Oto pełna treść rekomendacji:

* **Dynamiczny rozwój i skuteczność marketingu:** Kajo Data Space odnotowuje stały wzrost, z kwartału na kwartał docierając do coraz szerszego grona odbiorców. Rosnące przychody świadczą o wysokiej jakości usług oraz skuteczności prowadzonych działań marketingowych i promocyjnych. Obecny model pozyskiwania klientów wykazuje bardzo wysoką efektywność.

* **Najliczniejsza grupa to nowi klienci:** Analiza ogólna potwierdza wnioski z analizy kohortowej: największy udział w przychodach mają nowi klienci, którzy jednak szybko rezygnują z subskrypcji. Kluczowym priorytetem dla dalszego skalowania biznesu powinno być wdrożenie mechanizmów zatrzymujących użytkowników na dłużej, aby ustabilizować bazę stałych klientów.

## Przegląd ogólny klientów - Padsumowanie 

<img width="956" height="537" alt="Strona 2-1" src="https://github.com/user-attachments/assets/1cf9ee2b-31e7-4d17-8ff7-74684cb681d4" />

## Przegląd ogólny klientów - Rekomendacje 

<img width="962" height="542" alt="Strona 2-2" src="https://github.com/user-attachments/assets/b3626f6e-3250-42a4-b49e-4ba69db7a937" />


















