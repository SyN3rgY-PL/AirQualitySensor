# AirQualitySensor

## Opis kodu

Projekt `AirQualitySensor` to aplikacja Python służąca do monitorowania jakości powietrza przy użyciu czujników PM i BME280. Zapewnia zbieranie, przetwarzanie i dystrybucję danych o jakości powietrza.

## Kluczowe elementy kodu

### Klasa `AirQualitySensor`

Główna klasa skryptu, która zarządza procesem pomiaru, przetwarzania i dystrybucji danych.

#### Funkcje:
- Inicjalizacja komunikacji z czujnikami.
- Odczyt danych z czujnika BME280.
- Zarządzanie komendami i odczytem danych z czujnika PM.
- Ładowanie konfiguracji, zapis i wysyłka danych.

### Mechanizm kalibracji BME280

Kalibracja czujnika BME280 jest kluczowa dla uzyskania dokładnych pomiarów ciśnienia atmosferycznego. Skrypt uwzględnia kalibrację wysokości nad poziomem morza, co pozwala na precyzyjne dostosowanie ciśnienia do lokalnych warunków.

### Obsługa plików konfiguracyjnych JSON

Aplikacja wymaga plików konfiguracyjnych JSON dla ustawień połączenia z serwerem FTP (`ftp.json`) oraz bazą danych MySQL (`sql.json`). Użytkownik powinien dostosować te pliki do swoich potrzeb, wprowadzając odpowiednie dane dostępowe i parametry.

### Obsługa baz danych

Skrypt jest kompatybilny z różnymi systemami baz danych, w tym InfluxDB, Redis, MongoDB oraz PostgreSQL. Zapewnia to elastyczność w wyborze odpowiedniego rozwiązania do przechowywania i zarządzania danymi pomiarowymi.

### Pętla pomiarowa

Metoda `run_measurement_loop` zarządza cyklicznym procesem pomiarów, zapewniając odczyt, przetwarzanie i dystrybucję danych.

## Bezpieczeństwo i utrzymanie

Zalecane jest regularne aktualizowanie zależności, monitorowanie logów i sprawdzanie stanu czujników, oraz regularne tworzenie backupów.

## Wsparcie

W przypadku problemów lub pytań, zapraszamy do kontaktu przez zakładkę Issues w repozytorium GitHub.
