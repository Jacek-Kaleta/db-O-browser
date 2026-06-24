# DB (O) Browser — Oracle Schema Explorer

**DB (O) Browser** to szybka, lekka i w 100% lokalna aplikacja webowa (Single Page Application) służąca do przeglądania, eksploracji oraz analizy struktury schematów baz danych Oracle. 

Narzędzie działa w modelu **offline-first** – wszystkie operacje, parsowanie i wyszukiwanie odbywają się bezpośrednio w Twojej przeglądarce. Twoje dane strukturalne i metadane bazy nie są wysyłane na żaden zewnętrzny serwer, co zapewnia pełne bezpieczeństwo i poufność danych firmowych.

---

## 🚀 Główne Funkcje

- **Wbudowane skrypty eksportujące:** Aplikacja zawiera gotową paczkę skryptów SQL (`.zip`), które wystarczy uruchomić na bazie Oracle (np. przez SQL Developer), aby wyeksportować strukturę schematu do arkuszy Excela (`.xlsx`).
- **Wczytywanie Drag & Drop:** Wystarczy przeciągnąć i upuścić pliki `.xlsx` lub spakowane archiwum `.zip` bezpośrednio do okna aplikacji.
- **Błyskawiczne wyszukiwanie:** Zaawansowana wyszukiwarka z filtrami (Tabele, Widoki, Kolumny, Indeksy) i podświetlaniem szukanej frazy w czasie rzeczywistym.
- **Eksplorator obiektów (Sidebar):** Wygodne drzewo obiektów z podziałem na właścicieli (*Owners/Schemas*) oraz typy obiektów, z możliwością płynnej zmiany szerokości panelu.
- **Wielozakładkowy widok szczegółów:**
  - **Properties:** Podstawowe metadane obiektu.
  - **Columns:** Szczegółowa lista kolumn (typy danych jako kolorowe badge, statusy `NULL` / `NOT NULL` oraz oznaczenia kluczy głównych `PK`).
  - **Source Code:** Podgląd kodu źródłowego widoków czy procedur z numerowaniem linii.
  - **Relations (FK):** Wizualizacja relacji między tabelami wraz z automatycznym generowaniem gotowych zapytań `JOIN`.
- **Lokalna pamięć (IndexedDB):** Możliwość zapisania wczytanej struktury w pamięci przeglądarki, dzięki czemu nie trzeba ponownie wczytywać plików przy kolejnym uruchomieniu.
- **Wbudowany system logów:** Zaawansowany moduł diagnostyczny pomagający kontrolować poprawność parsowania plików.
- **Nowoczesny interfejs:** Wsparcie dla motywu jasnego oraz ciemnego (🌙), autorski system powiadomień toast oraz responsywny układ dostosowany do pracy z kodem.

---

## 🛠️ Architektura i Technologie

Projekt został zbudowany jako **Single Page Application (SPA)** zawarta w jednym, autonomicznym pliku HTML. Dzięki temu aplikację można uruchomić na dowolnym komputerze, po prostu klikając dwukrotnie w plik `db_browser.html`.

- **Frontend:** Czysty JavaScript (Vanilla JS), HTML5, CSS3 (zmienne CSS, Flexbox).
- **Zewnętrzne biblioteki (ładowane przez CDN):**
  - [SheetJS (xlsx.full.min.js)](https://github.com/SheetJS/sheetjs) – parsowanie arkuszy Excel w przeglądarce.
  - [JSZip (jszip.min.js)](https://github.com/Stuk/jszip) – dekompresja i tworzenie paczek ZIP.
- **Czcionki programistyczne:** Zastosowano fonty monospaced (*JetBrains Mono*, *Fira Code*) dla zwiększenia czytelności struktur SQL.

---

## 💻 Jak zacząć?

1. **Uruchom aplikację:** Pobierz i otwórz plik `db_browser.html` w dowolnej nowoczesnej przeglądarce internetowej.
2. **Pobierz skrypty SQL:** W sekcji powitalnej aplikacji kliknij przycisk pobierania paczki skryptów SQL.
3. **Wygeneruj raport z bazy:** Uruchom pobrane skrypty na swojej bazie Oracle za pomocą ulubionego klienta (np. Oracle SQL Developer) i zapisz wyniki jako pliki `.xlsx`.
4. **Wczytaj dane:** Przeciągnij wygenerowane pliki Excel (lub spakowany plik ZIP) do aplikacji i ciesz się błyskawicznym oraz wygodnym przeglądaniem bazy danych!

---

## 🤖 Informacja o projekcie

Aplikacja została zaprojektowana i wdrożona **przy współpracy z zaawansowaną sztuczną inteligencją (AI)**. Dzięki synergii ludzkiej wiedzy domenowej z zakresu baz danych oraz możliwości generatywnych AI, udało się stworzyć wysoce zoptymalizowane, bezpieczne i pozbawione ciężkiego backendu narzędzie typu *utility*, idealne do codziennej pracy deweloperów, analityków danych i administratorów baz danych Oracle.

---

## 📄 Licencja

Projekt udostępniany jest na licencji MIT. Szczegóły znajdziesz w pliku LICENSE.
