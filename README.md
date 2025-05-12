# Zadanie 1 w ramach LABORATORIUM: Programowanie Aplikacji w Chmurze Obliczeniowej

Aplikacja serwerowa napisana w C "server.c", oraz plik tworzący obraz "Dockerfile"
Sprawozdanie z zadania, znajduje się w pliku "zadanie1.md"

### Budowa obrazu

Polecenie

```
Docker build -t weather-server .
```

### Uruchomienie kontenera na podstawie zbudowanego obrazu

Polecenie

```
Docker run -d --name weather-server --rm -p 8080:8080 weather-server
```

Lub ręczne uruchomienie kontenera za pomocą aplikacji Docker desktop 

### Uzyskanie informacji z logów wygenerowanych w czasie powstania kontenera

Polecenie

``` 
Docker weather-server logs 
```

Lub mozliwość sprawdzenia logów w kontenerze w aplikacji Docker desktop

### Sprawdzenie rozmiaru oraz ilości warstw obrazu

Sprawdzenie ilości warstw:

```
docker inspect IMAGE_ID
```

Gdzie IMAGE_ID można sprawdzić po stworzeniu obrazu za pomocą polecenia

``` 
docker images 
```
 lub 
``` 
docker image ls 
```
