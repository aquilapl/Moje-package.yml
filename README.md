# Solus `package.yml` Collection

Kolekcja nieoficjalnych i zebranych plików konfiguracyjnych `package.yml` do budowania pakietów w systemie Solus OS.

## Jak użyć wybranego pliku?

Pliki w tym repozytorium posiadają nazwy w formacie `[nazwa_pakietu].package.yml`. 

Aby zbudować konkretny pakiet:

1. Pobierz wybrany plik.
2. Zmień jego nazwę na `package.yml` (zostawiając samą właściwą nazwę pliku).
3. Uruchom budowanie w profilu `unstable-x86_64`:

```bash
# Przykład dla clamav:
cp clamav.package.yml package.yml
sudo solbuild build package.yml -p unstable-x86_64
