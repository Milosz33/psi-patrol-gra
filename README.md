# PSI Patrol: Przygodowe Miasto 🐾

Fanowska, nieoficjalna gra platformowa 2D inspirowana serialem **PSI Patrol**. Cała grafika jest rysowana wektorowo w Canvasie (bez zewnętrznych plików graficznych) — jeden plik `index.html`, bez żadnych zależności ani instalacji.

## Jak uruchomić

Wystarczy otworzyć `index.html` w przeglądarce, albo wystawić go przez GitHub Pages (Settings → Pages → branch `main`, folder `/`).

## Rozgrywka

- Wybierz jednego z 6 psiaków — każdy ma inną zdolność specjalną:
  - **Chase** — susz start (krótki boost prędkości + chwilowa nietykalność)
  - **Marshall** — odporność na ogień + fala wody odpychająca wrogów
  - **Skye** — podwójny skok / szybowanie
  - **Rubble** — natychmiastowe wyburzanie skrzyń na drodze
  - **Rocky** — stawia tymczasową platformę nad przepaścią
  - **Zuma** — błyskawiczne pływanie, ignoruje prąd wody
- 4 tematyczne poziomy: Przygodowe Miasto, Farma Farmera Yumiego, Górska Kraina Jake'a, Plaża i Ocean
- Zbieraj kości (punkty) i ratuj zaginione kotki (misja poboczna → gwiazdki)
- 3 życia, przeciwnicy pokonywani skokiem na nich (jak w klasycznych platformówkach)
- System gwiazdek (1-3) i zapisany postęp między sesjami (localStorage)
- Sterowanie klawiaturą (strzałki/WASD, spacja = skok, Shift/E = zdolność, Esc = pauza) oraz przyciski dotykowe na urządzeniach mobilnych
- Dźwięki generowane w locie przez Web Audio API (bez plików audio)

## Struktura

```
index.html   – cała gra (HTML + CSS + JS w jednym pliku)
README.md    – ten plik
```

## Rozwój

Poziomy zdefiniowane są jako dane (`makeLevels()` w `index.html`) — platformy, wrogowie, przeszkody, kości i kotki to proste obiekty w tablicach, więc łatwo dodać kolejny poziom lub zmodyfikować istniejący bez ruszania silnika gry.

---
*Nieoficjalny projekt fanowski. PSI Patrol / PAW Patrol są znakami towarowymi ich właścicieli — ta gra nie jest z nimi powiązana ani przez nich sponsorowana.*
