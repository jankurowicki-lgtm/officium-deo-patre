# Officium Parvum de Deo Patre

Prosta aplikacja webowa/PWA do czytania historycznego *Officium Parvum de Deo Patre* na telefonie i komputerze.

## Co zawiera

- siedem godzin: Matutinum, Prima, Tertia, Sexta, Nona, Vesperae, Completorium;
- tekst łaciński oraz dodatkową *Oblatio* po Komplecie;
- trzy motywy: ciemny, jasny i sepia;
- regulację wielkości tekstu;
- zapamiętywanie ostatnio wybranej godziny i ustawień;
- tryb skupienia;
- podstawowy cache offline przez Service Worker;
- układ responsywny, przystosowany do telefonu.

## Uruchomienie lokalne

Nie otwieraj `index.html` jako `file://`, jeśli chcesz testować PWA/offline. Uruchom prosty serwer, np. w katalogu projektu:

```bash
python -m http.server 8000
```

Następnie otwórz `http://localhost:8000`.

## Publikacja przez GitHub Pages

1. Utwórz nowe repozytorium na GitHubie.
2. Wgraj wszystkie pliki i katalog `icons`.
3. Wejdź w **Settings → Pages**.
4. Wybierz **Deploy from a branch**, gałąź `main`, katalog `/ (root)`.
5. Zapisz ustawienia i poczekaj na publikację.
6. Otwórz adres GitHub Pages w Chrome na telefonie.

GitHub Pages udostępnia stronę przez HTTPS, co jest wymagane dla Service Workera i instalacji PWA.

## Instalacja na Redmi Note 15 Pro+ (Android)

1. Otwórz opublikowany adres strony w Chrome.
2. Poczekaj, aż strona załaduje się przynajmniej raz (to zapisuje pliki do cache).
3. Otwórz menu Chrome (⋮).
4. Wybierz **Zainstaluj aplikację** albo **Dodaj do ekranu głównego** (nazwa może zależeć od wersji Chrome/HyperOS).
5. Potwierdź. Ikona pojawi się na ekranie głównym i aplikacja będzie uruchamiana w osobnym oknie.

To jest PWA, a nie natywny plik APK. Do czytania oficjum, działania offline i uruchamiania z ekranu głównego nie jest potrzebny osobny APK.

## Źródło tekstu i uwagi redakcyjne

Transkrypcja łacińska została przygotowana na podstawie publikacji:
[Miles Christi Resístens — Oficio Parvo a Dios Padre](https://wwwmileschristi.blogspot.com/2020/08/oficio-parvo-dios-padre.html).

Wpis wskazuje jako źródło *Officium Rakocziánum*, skompilowane w 1836 r. Zachowano historyczną rubrykę dotyczącą Septuagesimy. Nie należy jej traktować jako automatycznej instrukcji dla aktualnego kalendarza liturgicznego.

**Ważne:** aplikacja nie jest oficjalną księgą liturgiczną ani publikacją zatwierdzoną przez władzę kościelną. Przed publicznym rozpowszechnianiem warto porównać transkrypcję z egzemplarzem źródłowym. W szczególności należy sprawdzić warianty pisowni, akcenty i interpunkcję. Nie dodano polskiego tłumaczenia modlitw, aby nie przedstawiać niezweryfikowanego przekładu jako historycznego tekstu.

## Licencja

Kod aplikacji można objąć licencją MIT po decyzji autora repozytorium. Nie oznacza to automatycznie, że transkrypcja, skan lub opracowanie tekstu źródłowego na stronie, z której korzystano, mają tę samą licencję. Przed publikacją sprawdź prawa do wykorzystanej transkrypcji i podaj wymagane atrybucje.
