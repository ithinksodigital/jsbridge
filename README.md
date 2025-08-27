# JSBridge Message Handler

Prosta strona HTML do obsługi wiadomości z JSBridge.

## Zawartość

- `index.html` - strona z obsługą JSBridge
- JSBridge Message Handler - odbiera i wyświetla wiadomości z różnych źródeł JSBridge

## Wdrożenie na GitHub Pages

### Krok 1: Utwórz nowe repozytorium na GitHub

1. Przejdź na [GitHub](https://github.com)
2. Kliknij "New repository"
3. Nazwij repozytorium (np. `jsbridge-handler`)
4. Zostaw je jako publiczne
5. Nie inicjalizuj z README (już mamy plik)

### Krok 2: Wgraj pliki do repozytorium

```bash
# Sklonuj repozytorium lokalnie
git clone https://github.com/TWOJA_NAZWA_UZYTKOWNIKA/jsbridge-handler.git
cd jsbridge-handler

# Skopiuj pliki do folderu
# (skopiuj index.html i README.md do tego folderu)

# Dodaj pliki do git
git add .

# Zatwierdź zmiany
git commit -m "Dodaj JSBridge message handler"

# Wypchnij na GitHub
git push origin main
```

### Krok 3: Włącz GitHub Pages

1. Przejdź do ustawień repozytorium (Settings)
2. Przewiń do sekcji "Pages"
3. W "Source" wybierz "Deploy from a branch"
4. Wybierz branch "main" i folder "/ (root)"
5. Kliknij "Save"

### Krok 4: Dostęp do strony

Twoja strona będzie dostępna pod adresem:
`https://TWOJA_NAZWA_UZYTKOWNIKA.github.io/jsbridge-handler`

## JSBridge Message Handler

Strona obsługuje wiadomości z różnych źródeł JSBridge:

### Obsługiwane źródła:
- **postMessage** - standardowe wiadomości WebView
- **webkit.messageHandlers** - iOS WKWebView
- **window.Android** - Android WebView
- **ReactNativeWebView** - React Native WebView
- **Custom Events** - niestandardowe zdarzenia

### Funkcje:
- Automatyczne wykrywanie dostępnych interfejsów JSBridge
- Wyświetlanie wiadomości w czasie rzeczywistym
- Licznik otrzymanych wiadomości
- Formatowanie JSON i stringów
- Ograniczenie do 50 ostatnich wiadomości
- Pasywne nasłuchiwanie - nie wymaga interakcji użytkownika

### Testowanie:
- Strona automatycznie odbiera wiadomości z aplikacji
- Można wywołać w konsoli: `jsbridgeHandler.testMessage()` (opcjonalnie)

## Sprawdzenie działania

1. Otwórz stronę w przeglądarce
2. Otwórz Developer Tools (F12)
3. Sprawdź konsolę - powinieneś zobaczyć komunikat "JSBridge handler initialized"
4. Gdy aplikacja wyśle wiadomość przez JSBridge, zostanie ona wyświetlona na stronie

## Uwagi

- Upewnij się, że repozytorium jest publiczne
- GitHub Pages może potrzebować kilku minut na wdrożenie
- Strona jest gotowa do użycia z aplikacjami mobilnymi i WebView # jsbridge
# jsbridge
