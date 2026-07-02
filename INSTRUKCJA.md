# Co Cię boli — wdrożenie na GitHub Pages

## Pliki w paczce
- `index.html` — cała aplikacja w jednym pliku (dane, styl, silnik)
- `manifest.webmanifest` — metryczka PWA (nazwa, kolory, ikony)
- `sw.js` — service worker: dzięki niemu apka działa offline
- `icon-192.png`, `icon-512.png` — ikonka na ekran telefonu

## Wdrożenie (raz, ~3 minuty)
1. Na GitHubie: **New repository**, nazwa np. `co-cie-boli`, publiczne.
2. **Add file → Upload files** → przeciągnij WSZYSTKIE 5 plików do katalogu głównego → Commit.
3. **Settings → Pages → Source: Deploy from a branch → Branch: main, folder: / (root) → Save.**
4. Po ~1 minucie apka działa pod adresem: `https://TWOJLOGIN.github.io/co-cie-boli/`

## Instalacja na telefonie (dla rodziny)
- **Android / Chrome:** otwórz link → menu ⋮ → „Dodaj do ekranu głównego” (czasem Chrome sam zaproponuje „Zainstaluj aplikację”).
- **iPhone / Safari:** otwórz link → przycisk Udostępnij (kwadrat ze strzałką) → „Do ekranu początkowego”.
- Po pierwszym otwarciu apka działa także **bez internetu**.

## Aktualizacje treści
1. Podmień `index.html` w repozytorium (Upload files → nadpisz).
2. W pliku `sw.js` podnieś numer w pierwszej linii: `ccb-v1` → `ccb-v2` (to każe telefonom pobrać świeżą wersję zamiast trzymać starą z pamięci).
3. Commit — po chwili wszyscy mają nową wersję.

## Uwaga
Repozytorium publiczne = treść apki jest publiczna (jak każda strona www).
