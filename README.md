# 📚 Angielski Fun - PWA do nauki słówek

Progresywna aplikacja webowa (PWA) do nauki angielskich słówek dla polskich dzieci (8+).

## ✨ Funkcje

- 📷 **OCR z zdjęcia** - Zrób zdjęcie ręcznie napisanej listy słówek, a aplikacja automatycznie ją rozpozna
- 📝 **Zarządzanie słówkami** - przeglądaj, edytuj, usuwaj i dodawaj nowe słówka
- 🎮 **Tryb quizu** - sprawdź swoją wiedzę z losowymi pytaniami
- 🔊 **Tekst na mowę** - słuchaj wymowy angielskich słówek
- 🎵 **Dźwięki** - efekty dźwiękowe przy odpowiedziach
- 📱 **PWA** - działa offline, można dodać do ekranu głównego

## 🚀 Jak uruchomić

### Lokalnie (najszybsze testowanie)

1. Otwórz plik `index.html` w przeglądarce (Chrome, Safari, Edge)
2. Gotowe! Aplikacja działa bez serwera

### Na telefonie

#### Opcja 1: GitHub Pages (polecane)

1. Stwórz nowe repozytorium na GitHub
2. Wgraj pliki: `index.html`, `manifest.json`, `sw.js`
3. Włącz GitHub Pages w ustawieniach repozytorium
4. Otwórz link na telefonie
5. Dodaj do ekranu głównego:
   - **iPhone (Safari)**: Share → Add to Home Screen
   - **Android (Chrome)**: Menu → Add to Home Screen

#### Opcja 2: Lokalny serwer

```bash
# Przejdź do folderu z aplikacją
cd vocab-pwa

# Python 3
python -m http.server 8000

# Node.js
npx serve .

# PHP
php -S localhost:8000
```

Następnie otwórz `http://localhost:8000` w przeglądarce.

## 📋 Format listy słówek do OCR

Aplikacja rozpoznaje różne formaty:
- `english word | polskie słowo`
- `english word - polskie słowo`
- `english word, polskie słowo`

Przykład:
```
cook | gotować
jump | skakać
swim | pływać
```

## 🧪 Przykładowe dane

Aplikacja zawiera przycisk "Wczytaj przykładowe słówka" z następującymi danymi:

**Czynności:**
- act / grać
- climb / wspinać się
- cook / gotować
- dive / nurkować
- draw / rysować
- fix / naprawiać
- jump / skakać
- read / czytać
- ride / jeździć
- run / biegać
- sing / śpiewać
- swim / pływać
- write / pisać

**Zwroty:**
- make a poster / zrobić plakat
- play football / grać w piłkę nożną
- ride a bike / jeździć na rowerze

## 🛠️ Technologie

- HTML5 + CSS3 + Vanilla JavaScript
- Tesseract.js (OCR)
- Web Speech API (text-to-speech)
- Web Audio API (efekty dźwiękowe)
- LocalStorage (zapisywanie danych)
- Service Worker (offline mode)

## 📱 Wymagania

- Nowoczesna przeglądarka (Chrome 60+, Safari 12+, Firefox 60+, Edge 79+)
- Dostęp do kamery (opcjonalnie, dla OCR)
- Internet (tylko przy pierwszym uruchomieniu, do pobrania Tesseract.js)

## 📝 Dane są zapisywane lokalnie

Wszystkie słówka są zapisywane w przeglądarce (localStorage). Nie są wysyłane na żaden serwer - prywatność jest zachowana!

## 🎨 Dostosowanie

Możesz zmienić kolory w sekcji `<style>` w `index.html`:
- `#667eea` - główny kolor (fioletowy)
- `#ff6b6b` - akcent (czerwony)
- `#4CAF50` - sukces (zielony)

## 📄 Licencja

MIT - wolne do użytku i modyfikacji!

---

Stworzone z ❤️ dla małej polskiej uczennicy uczącej się angielskiego!
