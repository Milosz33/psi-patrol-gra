# PSI Patrol: Ratunkowa Misja 🐾

Fanowska, nieoficjalna gra 2D z widokiem z góry, inspirowana serialem **PSI Patrol**. Prowadzisz pojazd wybranego psiaka po mapie i ratujesz Przygodowe Miasto — to gra jazdy/eksploracji, a nie platformówka skacząca po klockach. Cała grafika jest rysowana wektorowo w Canvasie z gradientami i cieniami (bez zewnętrznych plików graficznych) — jeden plik `index.html`, bez żadnych zależności ani instalacji.

## Jak uruchomić

Wystarczy otworzyć `index.html` w przeglądarce, albo wystawić go przez GitHub Pages (Settings → Pages → branch `main`, folder `/`).

## Rozgrywka

- Wybierz jednego z 6 psiaków i jego pojazd — każdy ma inną zdolność specjalną:
  - **Chase** (radiowóz) — syrena: krótki zryw prędkości + chwilowa nietykalność
  - **Marshall** (wóz strażacki) — armatka wodna: gasi ogniska, odpycha zagrożenia
  - **Skye** (helikopter) — tryb lotu: lata nad przeszkodami i wodą
  - **Rubble** (spycharka) — natychmiast rozjeżdża skrzynie i głazy
  - **Rocky** (ciężarówka recyklingu) — stawia tymczasową przeprawę przez wodę/błoto
  - **Zuma** (poduszkowiec) — błyskawiczny w wodzie, dodatkowy zryw na lądzie
- 4 tematyczne mapy: Przygodowe Miasto, Farma Farmera Yumiego, Górska Kraina Jake'a, Plaża i Ocean
- Zbieraj kości (punkty) i ratuj zaginione kotki (misja poboczna → gwiazdki)
- 3 życia, przeszkody blokują drogę, zagrożenia (ogień, wędrujące zwierzaki) odbierają życie
- System gwiazdek (1-3) i zapisany postęp między sesjami (localStorage)
- Sterowanie: strzałki/WASD (gaz/hamulec/skręt), Shift/E = zdolność, Esc = pauza, oraz przyciski dotykowe na urządzeniach mobilnych
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
