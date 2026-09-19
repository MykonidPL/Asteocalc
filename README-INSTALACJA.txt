ASTROCALC — INSTALACJA JAKO APLIKACJA NA ANDROIDZIE

Pakiet zawiera:
- index.html — aplikacja
- manifest.webmanifest — dane instalacyjne PWA
- service-worker.js — tryb offline
- icon-192.png i icon-512.png — ikony

WAŻNE
PWA musi być uruchomiona z adresu HTTPS (np. GitHub Pages). Samo otwarcie index.html z pamięci telefonu przez file:// nie daje pełnej instalacji PWA i service workera.

NAJPROSTSZA ŚCIEŻKA: GITHUB PAGES
1. Utwórz nowe publiczne repozytorium na GitHub, np. astrocalc.
2. Wgraj do katalogu głównego repozytorium wszystkie 5 plików aplikacji (bez konieczności wgrywania ZIP-a):
   index.html
   manifest.webmanifest
   service-worker.js
   icon-192.png
   icon-512.png
3. W repozytorium otwórz Settings > Pages.
4. W sekcji Build and deployment wybierz Deploy from a branch.
5. Branch: main, folder: /(root), następnie Save.
6. GitHub poda adres HTTPS strony. Otwórz go w Chrome na Androidzie.
7. Naciśnij przycisk „Zainstaluj” w AstroCalc. Jeśli go nie ma, użyj menu Chrome i wybierz instalację/dodanie do ekranu głównego.
8. Po instalacji AstroCalc pojawi się jako ikona na pulpicie i będzie uruchamiać się w osobnym oknie.
9. Otwórz aplikację przynajmniej raz z internetem; potem zasoby aplikacji są dostępne offline.

AKTUALIZACJA
Gdy podmienisz pliki na GitHub Pages, przeglądarka pobierze nową wersję. Jeśli zmieniasz service-worker.js i chcesz wymusić odświeżenie cache, zmień nazwę CACHE, np. astrocalc-v1 -> astrocalc-v2.
