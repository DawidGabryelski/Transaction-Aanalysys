# Kajo Data Space - Analiza sprzedaży

## 1. Cele projektu i opis

Jest to projekt konkursowy który skupia się na analizie danych transakcyjnych KajoDataSpace od początku jego istnienia. Projekt zawiera dwie strony. 
Retencja w ujęciu kohortowym oraz przegląd ogólny klientów.

## 2. Retencja w ujęciu kohortowym

Ta strona składa się z pięciu elementów:

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

#### d1) Dynamiczne pole tekstowwe  

Pole tekstowe które zawiera dynamiczny tekst który dostosowywuje się do wartości filtra. Możemy tam znaleźć informację o wybranej grupie, jej stanie początkowym, przychodzie wygenerowanym przez
całą tą grupę liczbie pozostałych klientów, oraz liczbie klientów będących od momentu dołączenia (wybrany filtr) do dnia dzisiejszego - 31.03.2026

#### d2) Rekomendacje 

To pole zawiera rekomendacje dla odbiorcy - jeden z wymogów konkursowych.Oto pełna treść rekomendacji:

* Ucieczka po miesiącu: Analiza kohortowa wskazuje, że większość nowych klientów rezygnuje już po pierwszym miesiącu.
Zaleca się wprowadzenie atrakcyjnych planów 3-miesięcznych, oferujących wyższy rabat niż plan miesięczny. Pozwoli to klientom na
dłuższą perspektywę zapoznania się z treściami, przy jednoczesnym uniknięciu bariery wysokiego kosztu planu rocznego.

* Co zrobić z powracającymi klientami?: W celu aktywacji powracających użytkowników rekomendowane jest wprowadzenie zniżek motywacyjnych.
Warunkiem otrzymania rabatu powinno być wypełnienie krótkiego formularza. Pozwoli to na zebranie cennych danych o przyczynach 
wcześniejszych rezygnacji i pomoże w optymalizacji usługi w przyszłości.

### Retencja w ujęciu kohortowym - Bez aktywnego filtra 

<img width="958" height="537" alt="Strona 1-1" src="https://github.com/user-attachments/assets/39f7121f-8936-4435-8dfd-12a612be43d2" />

### Retencja w ujęciu kohortowym - Aktywny flitr

<img width="962" height="541" alt="Strona 1-2" src="https://github.com/user-attachments/assets/8009e3ca-86e7-4a79-bada-3a18d7f2e366" />

### Retencja w ujęciu kohortowym - Zakładka rekomendacje

<img width="957" height="536" alt="Strona 1-3" src="https://github.com/user-attachments/assets/108b273d-7f6a-4413-9eeb-5e286a794677" />














