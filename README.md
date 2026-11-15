# Ziemia Wrocław

Jednostronicowa strona internetowa promująca sprzedaż ziemi i kruszyw na terenie Wrocławia i okolic.

## Struktura katalogów

- `index.html` – główna struktura strony
- `assets/css/styles.css` – arkusz stylów
- `assets/js/script.js` – małe skrypty interaktywne
- `assets/images/` – zdjęcia wykorzystane na stronie

## Jak uruchomić stronę lokalnie

1. Otwórz folder projektu w dowolnym edytorze.
2. Uruchom prosty serwer lokalny z poziomu katalogu projektu:

```bash
python -m http.server 8000
```

3. Otwórz w przeglądarce adres:

```text
http://localhost:8000
```

## Jak zmienić numer telefonu

Wprowadź numer telefonu w następujących miejscach w pliku `index.html`:

- przycisk `Zadzwoń teraz` w nagłówku
- przycisk `Zadzwoń teraz` w sekcji kontaktu
- linki `tel:` w sekcji hero i transportu

Przykład:

```html
<a href="tel:+48000000000">Zadzwoń teraz</a>
```

Wystarczy podmienić wartość po `tel:` na właściwy numer.

## Jak zmienić teksty

Edytuj treści bezpośrednio w pliku `index.html`.

Najważniejsze fragmenty do personalizacji:

- nazwa marki
- nagłówek hero
- opis oferty
- treść sekcji transportu
- kontakty i stopka

## Jak podmienić zdjęcia

1. Zamiast obecnych plików w katalogu `assets/images/` wstaw nowe zdjęcia o podobnym rozmiarze i proporcji.
2. Zachowaj nazwy plików albo zaktualizuj ścieżki w `index.html`:

```html
<img src="assets/images/hero-soil.jpg" alt="Ziemia ogrodowa" />
```

Dobrze jest przechowywać zdjęcia w jednym katalogu, aby późniejsza wymiana była szybka i bezproblemowa.

## Jak przygotować stronę do publikacji na hostingu

1. Upewnij się, że wszystkie pliki są w katalogu głównym projektu.
2. Zadbaj o to, aby w katalogu `assets` znajdowały się CSS, JS i obrazy.
3. Prześlij całą zawartość na hosting obsługujący statyczne strony HTML.
4. Ustaw główny plik wejściowy na `index.html`.
5. Po wdrożeniu sprawdź poprawność wyświetlania w przeglądarce.

## Wskazówki dotyczące dalszego rozwoju

- Numer telefonu i dane kontaktowe można łatwo zmienić w jednym pliku `index.html`.
- Kolory, odstępy i układ są zorganizowane w `assets/css/styles.css`.
- Strona została wykonana w technologii HTML/CSS/JS bez dodatkowych bibliotek, co ułatwia utrzymanie i wdrożenie.
