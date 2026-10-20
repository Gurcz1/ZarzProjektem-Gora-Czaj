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