# AirQualitySensor

## Opis Kodu

Projekt `AirQualitySensor` to aplikacja Python służąca do monitorowania jakości powietrza przy użyciu czujników PM i BME280. Zapewnia on zbieranie, przetwarzanie i dystrybucję danych o jakości powietrza.

## Kluczowe Elementy Kodu

### Klasa `AirQualitySensor`

Główna klasa skryptu, która zarządza procesem pomiaru, przetwarzania i dystrybucji danych.

#### Funkcje:
- Inicjalizacja komunikacji z czujnikami.
- Odczyt danych z czujnika BME280.
- Zarządzanie komendami i odczytem danych z czujnika PM.
- Ładowanie konfiguracji, zapis i wysyłka danych.

### Mechanizm Kalibracji BME280

Kalibracja czujnika BME280 jest kluczowa dla uzyskania dokładnych pomiarów ciśnienia atmosferycznego. Skrypt uwzględnia kalibrację wysokości nad poziomem morza, co pozwala na precyzyjne dostosowanie ciśnienia do lokalnych warunków. Użytkownik powinien dostosować parametry kalibracji do swojej lokalizacji, aby zapewnić najwyższą dokładność pomiarów.

### Pętla pomiarowa

Metoda `run_measurement_loop` zarządza cyklicznym procesem pomiarów, zapewniając odczyt, przetwarzanie i dystrybucję danych.

## Bezpieczeństwo i Utrzymanie

Zalecane jest regularne aktualizowanie zależności, monitorowanie logów i sprawdzanie stanu czujników, oraz regularne tworzenie backupów.

## Wsparcie

W przypadku problemów lub pytań, zapraszamy do kontaktu przez zakładkę Issues w repozytorium GitHub lub do poszukiwania odpowiedzi w społecznościach online Raspberry Pi, Pythona oraz DIY.
