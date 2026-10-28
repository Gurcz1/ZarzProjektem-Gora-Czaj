# Zarządzanie Projektem Informatycznym – Laboratoria
**Poziomy gotowości technologicznej: TRL 1 (Badania podstawowe)**

## 1. Skład zespołu projektowego
*   **Kierownik Projektu:** Jakub Góralski
*   **Analiza i koncepcja:** Patryk Czajowski

---

## 2. Opis koncepcji technologicznej (TRL 1)

### Główna idea i zaobserwowany potencjał
W wyniku analiz potrzeb społeczności studenckiej na kampusie Kortowo, zespół opracował koncepcję mobilnego systemu lokalizacyjno-społecznościowego o roboczej nazwie **KortoPifko**. Zauważono, że studenci szukający towarzystwa do wyjścia na piwo lub po prostu wspólnego spędzenia czasu na świeżym powietrzu, zmagają się z chaosem informacyjnym na tradycyjnych grupach dyskusyjnych.

Główna idea opiera się na stworzeniu dynamicznej mapy, na której użytkownik może postawić „pinezkę” informującą o tym, gdzie i kiedy planuje się spotkać i integrować. Inni ludzie widzą takie punkty w czasie rzeczywistym i mogą łatwo dołączyć do otwartej grupy, co maksymalnie upraszcza socjalizację i poznawanie nowych znajomych.

### Funkcjonalności i potencjalne zastosowania
Wstępna koncepcja zakłada, że system będzie oferował możliwości filtrowania i dopasowywania spotkań, które mogą być rozwijane w wyższych poziomach TRL:
*   **Filtry dopasowania:** Użytkownicy mogą określić swój kierunek, rok studiów, zainteresowania oraz typ alkoholu/napojów, jakie planują spożywać, co ułatwia znalezienie ludzi o podobnych preferencjach.
*   **Zastosowanie w obronności / zarządzaniu kryzysowym:** Moduł mapowania dużych skupisk ludzkich w czasie rzeczywistym posiada potencjał, który w przyszłości może zostać zaadaptowany przez służby porządkowe lub organizatorów imprez masowych (np. podczas Kortowiady) do monitorowania tłumu i zapewniania bezpieczeństwa na terenie kampusu.

## 3. Badania przemysłowe – TRL 2

### Zadanie 1. Koncepcja technologii i jej przyszłego zastosowania

Przeprowadzono wstępną analizę możliwych zastosowań technologii KortoPifko. Ustalono, że system najlepiej zrealizować jako **aplikację mobilną na Androida i iOS** z interaktywną mapą kampusu Kortowo, współpracującą z centralnym serwerem. Aplikacja ma być prosta i intuicyjna, zgodnie z zasadą: im mniej kliknięć do rezultatu, tym lepiej. Dodanie spotkania ma wymagać maksymalnie trzech kroków: wybór miejsca, godziny i typu spotkania.

Zaplanowano następujące komponenty:
- **mapa spotkań w czasie rzeczywistym**, z pinezkami pokazującymi miejsce, godzinę i liczbę dołączonych osób,
- **filtry dopasowania**: kierunek, rok studiów, zainteresowania i rodzaj spotkania,
- **rejestracja przez konto uczelniane**, aby ograniczyć użytkowników do społeczności UWM,
- **weryfikacja pełnoletności** oraz opcja spotkań bezalkoholowych (planszówki, sport, grill). Poszerza ona grupę docelową i ogranicza ryzyka wizerunkowe,
- **moduł bezpieczeństwa**: zgłaszanie nadużyć, blokowanie użytkowników i ochrona prywatności lokalizacji (zgodność z RODO).

Zastosowanie zostanie wstępnie ukierunkowane na integrację studentów UWM, a w dalszej kolejności na inne kampusy akademickie.

### Zadanie 2. Lista rzeczy potrzebnych do dalszego rozwoju projektu

**Infrastruktura i sprzęt**
- 3x komputer/laptop do programowania (min. 16 GB RAM),
- 1x komputer Mac do budowania i testowania wersji iOS,
- 3x smartfon testowy (w tym min. 1 iPhone),
- szybki dostęp do Internetu (łącze światłowodowe),
- środowisko testowe (serwer w chmurze/VPS) oraz baza danych.

**Oprogramowanie i usługi**
- 3x środowisko programistyczne (Android Studio, Xcode, VS Code),
- system kontroli wersji i zarządzania zadaniami (GitHub + Jira/Trello),
- narzędzie do projektowania interfejsu (Figma),
- usługa map (Google Maps API lub OpenStreetMap) i komunikacji w czasie rzeczywistym (Firebase/WebSocket),
- konta deweloperskie: Apple Developer i Google Play Console.

**Organizacyjne**
- konsultacja prawna w zakresie RODO i regulaminu aplikacji,
- grupa testowa studentów (min. 20 osób) do badań użyteczności,
- budżet na hosting i licencje API.

## 4. Badania przemysłowe – TRL 3

### Zadanie 1. Potwierdzenie analityczne i eksperymentalne założeń koncepcji

W ramach realizacji III poziomu gotowości technologicznej zostaną zrealizowane prace badawcze nad poszczególnymi komponentami systemu KortoPifko. Komponenty będą testowane osobno i nie będą jeszcze połączone w całość. Celem jest zebranie dowodów, że założenia przyjęte na poziomie TRL 2 są zasadne.

**Moduł mapy i pinezek w czasie rzeczywistym**
Zostanie sprawdzona możliwość wyświetlania na mapie kampusu Kortowo pinezek spotkań wraz z godziną i liczbą uczestników oraz ich aktualizacji w czasie rzeczywistym. Szczególny nacisk zostanie położony na opóźnienie między dodaniem pinezki przez jednego użytkownika a jej pojawieniem się u pozostałych. Zbadane zostanie też zużycie transferu danych i baterii w telefonie podczas ciągłego odświeżania mapy. W ramach badań zostanie porównane działanie dwóch dostawców map (Google Maps API oraz OpenStreetMap) pod kątem kosztów, dokładności i płynności działania.

**Moduł filtrów i dopasowania spotkań**
Moduł będzie filtrował spotkania według kierunku, roku studiów, zainteresowań i rodzaju spotkania. Zostanie zbadana poprawność i szybkość filtrowania przy rosnącej liczbie aktywnych pinezek. Zostanie także opracowany prosty model oceny trafności dopasowania, którego miarą końcową będzie odsetek propozycji ocenionych przez testerów jako trafne (wyrażony w procentach).

**Moduł rejestracji i weryfikacji użytkownika**
Zostanie zweryfikowana możliwość logowania kontem uczelnianym UWM, aby ograniczyć dostęp do społeczności uczelni. W module zostanie zbadana także weryfikacja pełnoletności użytkownika wymagana dla spotkań z alkoholem oraz czas i liczba kroków potrzebnych do pierwszej rejestracji.

**Moduł bezpieczeństwa i prywatności lokalizacji**
Zostaną zbadane mechanizmy zgłaszania nadużyć i blokowania użytkowników oraz ochrony prywatności. Lokalizacja użytkowników nie będzie udostępniana innym. Widoczne będą wyłącznie miejsca spotkań wskazane przez organizatorów. Zostanie przeprowadzona wstępna analiza zgodności z RODO (zakres przetwarzanych danych, czas ich przechowywania, zgody użytkownika).

**Badanie potrzeb użytkowników**
Zostanie przeprowadzona anonimowa ankieta wśród studentów kampusu Kortowo (zakładana próba: min. 50 osób). Ma ona potwierdzić, czy problem chaosu informacyjnego na grupach dyskusyjnych faktycznie występuje oraz czy studenci są zainteresowani aplikacją i spotkaniami bezalkoholowymi. Wyniki będą podstawą do dalszej oceny zasadności biznesowej projektu.

**Model matematyczny obciążenia**
Na poziomie wskazanego etapu zostanie określony model matematyczny szacujący obciążenie serwera w zależności od liczby jednocześnie aktywnych użytkowników, liczby pinezek i częstotliwości odświeżania mapy. Pozwoli on oszacować wymagane zasoby serwerowe i koszty hostingu przy skalowaniu systemu, np. podczas Kortowiady.

### Zadanie 2. Siedem pryncypiów metodyki PRINCE2 w projekcie KortoPifko

1. **Ciągła zasadność biznesowa** – na każdym etapie sprawdzamy, czy projekt ma sens. Wyniki ankiety i testów komponentów pokażą, czy warto go kontynuować. W razie braku uzasadnienia można go szybko zakończyć, ograniczając koszty. Kontrolujemy też ryzyka (np. wizerunkowe związane z alkoholem, RODO).
2. **Zdefiniowane role i odpowiedzialności** – najpierw określamy role, potem przypisujemy je osobom. Kierownik projektu (Jakub Góralski) koordynuje prace i nie łączy swojej roli z rolami komitetu sterującego.
3. **Koncentracja na produktach** – produktem jest aplikacja mobilna KortoPifko. Najpierw ustalamy jej definicję i kryteria jakości (np. dodanie spotkania w maks. 3 krokach), a potem rozkładamy drogę do celu na czynności.
4. **Korzystanie z doświadczeń** – wnioski z poprzednich laboratoriów i innych projektów uwzględniamy w kolejnych etapach (np. doprecyzowanie grupy docelowej i wykluczenie na razie zastosowania w obronności).
5. **Zarządzanie z wykorzystaniem tolerancji** – komitet sterujący wyznacza granice tolerancji (czas, koszt, a także jakość, zakres i ryzyko), w których kierownik może samodzielnie podejmować decyzje.
6. **Zarządzanie etapowe** – projekt dzielimy na etapy (kolejne poziomy TRL). Przejście do następnego wymaga zgody i potwierdzenia, że projekt nadal ma uzasadnienie biznesowe.
7. **Dostosowanie do projektu w danym środowisku** – metodykę i narzędzia dobieramy do skali projektu. Mały zespół studencki nie potrzebuje rozbudowanej dokumentacji, tylko „skrojonego” zestawu narzędzi.

## 5. Badania przemysłowe – TRL 4

### Zadanie 1. Weryfikacja koncepcji w warunkach laboratoryjnych.

W ramach realizacji IV poziomu gotowości technologicznej zostaną zrealizowane pracę badawcze w następującym zakresie:

- **Moduł mapy i pinezek w czasie rzeczywistym** – przygotowano zestaw kontrolny 100 punktów współrzędnych geograficznych odwzorowujących popularne miejsca spotkań w Kortowie (np. Plaża Kortowska, Górka Kortowska, Promenada). Wykonano po 100 serii testów dla zestawu kontrolnego. Algorytm wykazał pewne odchylenie, w niektórych seriach testów. Ustalono, że na wynik ma wpływ użycie funkcji lokalizacji w telefonie przy jednoczesnym generowaniu wielu punktów blisko siebie. Wprowadzono poprawkę do algorytmu (łączenie bliskich pinezek w jedną większą grupę oraz ograniczenie częstotliwości odświeżania pozycji) i ponownie wykonano 100 serii testów. Wyniki w całej serii były porównywalne, a odchylenia zostały zminimalizowane.

- **Moduł filtrów i dopasowania spotkań** – przygotowano zestaw kontrolny 100 profili studenckich z przypisanymi zmiennymi: kierunek studiów, rok oraz preferencje (np. planszówki, grill, piwo). Wykonano po 100 serii testów dla zestawu kontrolnego plików. Algorytm wykazał pewne odchylenie, w niektórych seriach testów. Ustalono, że na wynik ma wpływ użycie zbyt wielu filtrów jednocześnie, co zawieszało wyszukiwanie. Wprowadzono poprawkę do algorytmu poprzez uproszczenie sposobu przeszukiwania bazy danych spotkań i ponownie wykonano 100 serii testów. Wyniki w całej serii były porównywalne, a odchylenia zostały zminimalizowane.

- **Moduł rejestracji i weryfikacji użytkownika** – przygotowano zestaw kontrolny 100 testowych kont studenckich do uwierzytelniania w domenie UWM. Wykonano po 100 serii testów dla zestawu kontrolnego kont. Podczas każdego testu weryfikowano poprawność logowania. Algorytm wykazał pewne odchylenie, w niektórych seriach testów. Ustalono, że na wynik ma wpływ funkcja czasu trwania zalogowania użytkownika, która wylogowywała go w losowych momentach. Wprowadzono poprawkę do algorytmu poprawiając system podtrzymywania sesji w tle i ponownie wykonano 100 serii testów. Wyniki w całej serii były porównywalne, a odchylenia zostały zminimalizowane.

- **Moduł bezpieczeństwa i prywatności lokalizacji** – przygotowano zestaw kontrolny 100 symulowanych kont zgłaszających nadużycia oraz testowych zapytań o lokalizację. Wykonano po 100 serii testów dla zestawu kontrolnego. Algorytm wykazał pewne odchylenie, w niektórych seriach testów polegające na pokazywaniu dokładnego adresu zamieszkania użytkownika zamiast ogólnego punktu na mapie. Ustalono, że na wynik ma wpływ brak domyślnego ukrywania prywatnych współrzędnych. Wprowadzono poprawkę do algorytmu (wprowadzono mechanizm pokazywania przybliżonego okręgu obecności użytkownika zamiast dokładnej pinezki) i ponownie wykonano 100 serii testów. Wyniki w całej serii były porównywalne, a odchylenia zostały zminimalizowane.

### Zadanie 2. Ryzyka dla IV poziomu TRL i sposoby ich eliminacji

Ryzyka uszeregowano według prawdopodobieństwa wystąpienia (najwyższe są eliminowane w pierwszej kolejności).

**1. Ryzyko (40%):** Zawieszanie się interaktywnej mapy i wolne działanie aplikacji na starszych lub słabszych modelach smartfonów.
**Rozwiązanie:** Optymalizacja interfejsu graficznego oraz ładowanie danych o spotkaniach dopiero wtedy, gdy użytkownik przesunie mapę w dany obszar kampusu. Rozszerzenie testów o różne modele telefonów (Android i iOS).

**2. Ryzyko (35%):** Przeciążenie serwera przy dużej liczbie jednocześnie aktywnych użytkowników (np. podczas Kortowiady).
**Rozwiązanie:** Testy obciążeniowe na podstawie modelu matematycznego z TRL 3, buforowanie danych i ograniczenie częstotliwości odświeżania mapy.

**3. Ryzyko (30%):** Brak poprawnej komunikacji lub niekompatybilność danych pomiędzy modułami (mapa, filtry, logowanie).
**Rozwiązanie:** Zaprogramowane testy automatyczne oraz zastosowanie wzorca architektonicznego MVC (Model-View-Controller). Eliminacja błędów „krok po kroku".

**4. Ryzyko (20%):** Przypadkowe wyświetlenie dokładnej lokalizacji studenta zamiast miejsca spotkania (naruszenie prywatności i zasad RODO).
**Rozwiązanie:** Blokada systemowa uniemożliwiająca przesyłanie precyzyjnych współrzędnych użytkownika. Lokalizacja jest udostępniana tylko za wyraźną zgodą studenta.
