# Podstawy Uczenia Maszynowego - laboratoria

## Spis treści

* [Modele liniowe (linear models)](lab1)
* [Modele oparte o sąsiedztwo (nearest neighbors)](lab2)
* [Metody jądrowe (kernel methods)](lab3)
* [Metody probabilistyczne (probabilistic methods)](lab4)

## Setup

Zależności potrzebne do wykonania notebooków są zawarte w `pyproject.toml` oraz `uv.lock`,
zarządzanych przez [uv](https://docs.astral.sh/uv/). Jeżeli korzystasz z PyCharma, stwórz
nowy projekt z dependency managerem uv (File -> Settings -> Project -> Python interpreter
-> Add interpreter -> uv). Uruchomienie w terminalu `uv sync` zainstaluje odpowiednią wersję
Pythona oraz wszystkie zależności. Pliki będą systematycznie aktualizowane na potrzeby
kolejnych laboratoriów.

Aktualizacja zależności wymaga wywołania ponownie `uv sync`. W razie potrzeby przebudowania
zależności w uv trzeba dodać ją do `pyproject.toml` oraz rozwiązać i zainstalować zależności
przez `uv sync`.

Repozytorium zawiera też bibliotekę [ruff](https://docs.astral.sh/ruff/) do formatowania
kodu. Sugerowane jest użycie [pre-commit hooka](https://docs.astral.sh/ruff/integrations/#pre-commit),
przykładową konfigurację zawarto w `.pre-commit-config.yaml`.

## Zasady zaliczania laboratoriów

1. Jest 7 laboratoriów, z każdego laboratorium można otrzymać 10 punktów oraz ewentualnie punkty za zadanie dodatkowe, 
   niewchodzące do podstawowej puli.
2. Warunkiem zaliczenia indywidualnych ćwiczeń laboratoryjnych jest uzyskanie minimum 5 punktów z tych ćwiczeń. 
   Punkty za zadania dodatkowe są uwzględniane tylko wtedy, gdy uzyskano zaliczenie z każdych indywidualnych ćwiczeń.
3. Warunkiem uzyskania zaliczenia z przedmiotu jest zaliczenie wszystkich indywidualnych ćwiczeń laboratoryjnych.
4. Rozwiązanie indywidualnych ćwiczeń (z wyjątkiem ostatnich ćwiczeń) musi zostać wysłane na MS Teams w ciągu 2 tygodni 
   od laboratoriów, na których zostało zadane, do godz. 23:59, zgodnie z terminem podanym w zadaniu na MS Teams.
5. Na laboratoriach 2-7 będzie przeprowadzona pisemna kartkówka z tematyki poprzedniego laboratorium oraz zadania. Z każdej kartkówki 
   można otrzymać 5 punktów. Nie ma minimalnej liczby punktów, które trzeba uzyskać w ramach kartkówek.
6. Zgodnie z sylabusem, istnieje możliwość zamiany kartkówek na projekt indywidualny, w ramach którego należy zaimplementować 
   wybrany (i zaakceptowany przez prowadzącego) artykuł naukowy, oraz przygotować raport z jego wykonania i zaliczyć kolokwium 
   ustne na koniec semestru.
7. W przypadku spóźnienia się z oddaniem indywidualnych ćwiczenia można je wysłać ze spóźnieniem w ciągu kolejnych 2 tygodni. 
   Wtedy otrzymana liczba punktów jest mnożona przez 0.8, włącznie z ewentualnymi punktami za zadanie dodatkowe, zaokrąglona w górę 
   do najbliższego 0.25 punktu.
8. Zestaw zadań przesłany w terminie znacznie wcześniejszym niż podstawowy może zostać odesłany z sugestiami poprawek. Taki zestaw 
   może zostać przesłany ponownie, z uwzględnieniem tych poprawek. Zestawy przysłane blisko końca terminu oraz w terminie poprawkowym 
   mogą zostać wysłane tylko raz, tj. nie ma możliwości ich poprawiania czy dosyłania zadań.
9. Punkt o możliwości spóźnienia nie dotyczy sytuacji, w której student miał nieobecność nieusprawiedliwioną na zajęciach. 
   W takim wypadku zestaw z tego laboratorium, na którym student był nieobecny, można oddać jedynie w terminie podstawowym. W takiej 
   sytuacji z kartkówki (punkt 4) student otrzymuje zero punktów.
10. W ramach zadań mogą pojawić się odpowiednio oznaczone zadania dodatkowe. Punkty z tych zadań są dodatkowe, tj. wliczają się do 
   sumy uzyskanych punktów (licznika), ale nie do mianownika.
11. Zadania dodatkowe można dosłać w terminie podstawowym lub poprawkowym, nawet jeżeli został już wysłany podstawowy zestaw. Stanowi 
    to wyjątek od reguły z punktu 8. W przypadku przesłania go w terminie poprawkowym punkty są redukowane zgodnie z opisem w punkcie 7.
12. W przypadku nieuzyskania zaliczenia z co najmniej jednego z ćwiczeń indywidualnych (w szczególności uwzględniając minimum 
   punktowe z pkt. 2, oraz termin spóźniony z pkt. 5), w pierwszym terminie zaliczenia przedmiotu wystawiana jest ocena niedostateczna. 
13. W przypadku nieuzyskania zaliczenia w pierwszym terminie możliwe jest uzyskanie zaliczenia w terminie poprawkowym, jeśli
   wszystkie brakujące ćwiczenia indywidualne zostaną ocenione pozytywnie do końca sesji poprawkowej.
14. W przypadku uzyskania zaliczenia stosowana jest skala ocen AGH, tj.:
    * `50-59` pkt. - ocena 3 (dst)
    * `60-69` pkt. - ocena 3,5 (+dst)
    * `70-79` pkt. - ocena 4 (db)
    * `80-89` pkt. - ocena 4,5 (+db)
    * `>= 90` pkt. - ocean 5 (bdb)
15. Zgodnie z sylabusem, jeżeli pozytywną ocenę z laboratorium i zaliczenia wykładu uzyskano w pierwszym terminie 
    oraz ocena końcowa jest mniejsza niż 5.0 to ocena końcowa jest podnoszona o 0.5.
