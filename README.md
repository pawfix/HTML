# 🚀 Moja podróż w Web Development

> Repozytorium: `pawfix/HTML`\
> Cel: dokumentuję naukę frontendu (HTML/CSS/JS) i tworzę małe projekty krok po kroku.

---

## Spis treści

1. [O repozytorium](#o-repozytorium)
2. [Jak uruchomić](#jak-uruchomić)
3. [Struktura katalogów](#struktura-katalogów)
4. [Stack i narzędzia](#stack-i-narzędzia)
5. [Roadmapa nauki](#roadmapa-nauki)
6. [Dziennik postępów](#dziennik-postępów)
7. [Mini–projekty](#mini–projekty)
8. [Zasady jakości](#zasady-jakości)
9. [Zadania / To‑Do](#zadania--to-do)
10. [Jak kontrybuować](#jak-kontrybować)
11. [Licencja](#licencja)

---

## O repozytorium

To miejsce, gdzie:

- ćwiczę **HTML5**, **CSS3** i **JavaScript** od podstaw do projektów produkcyjnych,
- porównuję różne techniki (flex vs grid, vanilla JS vs framework),
- zapisuję notatki i dobre praktyki,
- buduję kolekcję mini–projektów (komponenty, layouty, mikro‑interakcje).

> 🔎 Tip: każdy folder projektu ma własny `README.md` z krótkim opisem, zrzutem ekranu i checklistą kryteriów jakości.

---

## Jak uruchomić

Najprościej — otwórz plik `index.html` wybranego projektu w przeglądarce.

**Opcja dev (serwer lokalny):**

```bash
# Python 3
python -m http.server 5173
# lub Node (jeśli masz)
npx serve . -l 5173
```

Następnie wejdź na `http://localhost:5173`.

---

## Struktura katalogów

Przykładowa struktura (może rosnąć w czasie):

```
HTML/
├─ 00-basics/           # absolutne podstawy (tagi, semantyka, formularze)
├─ 01-css-layouts/      # flexbox, grid, pozycjonowanie
├─ 02-components/       # karty, navbary, przyciski, formularze
├─ 03-js-fundamentals/  # DOM, zdarzenia, fetch, moduły
├─ 04-mini-projects/    # małe aplikacje (todo, kalkulator, timer)
├─ 05-accessibility/    # a11y: aria, focus, kontrast
├─ assets/              # obrazy, ikony, fonty
└─ docs/                # notatki, artykuły, zrzuty ekranu
```

> Jeśli w repo istnieje inny układ — z czasem dostosuję strukturę i zaktualizuję ten opis.

---

## Stack i narzędzia

- **Języki:** HTML5, CSS3 (Flex/Grid), JavaScript (ES202x)
- **Style & UI:** BEM, Utility‑First (opcjonalnie), animacje CSS
- **Narzędzia dev:** VS Code, Prettier, ESLint (dla JS), Live Server
- **Kontrola wersji:** Git + GitHub (konwencja commitów: *feat/fix/docs/refactor/chore*)

**Formatowanie kodu:**

```json
{
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "files.eol": "\n",
  "prettier.singleQuote": true,
  "prettier.semi": false
}
```

---

## Roadmapa nauki

1. **HTML Semantyczny** – nagłówki, listy, tabele, formularze, tagi `<section>`, `<article>`, `<nav>`, `<main>`.
2. **CSS Podstawy** – selektory, box model, typografia, kolory, zmienne CSS.
3. **Layouty** – Flexbox, Grid, responsywność (mobile‑first), media queries, *container queries*.
4. **Komponenty UI** – nawigacje, karty, formularze z walidacją, modale, tooltips.
5. **JavaScript** – DOM, zdarzenia, async/await, fetch API, lokalne storage, moduły ES.
6. **Dostępność (a11y)** – aria‑labels, focus states, kontrast, klikalność klawiaturą.
7. **Wydajność** – optymalizacja obrazów, lazy‑loading, minimalizacja CSS/JS.
8. **Jakość** – linting, formatowanie, testy (np. Playwright/Web‑Test w przyszłości).
9. **Publikacja** – GitHub Pages/Netlify, wersjonowanie, changelog.

---

## Dziennik postępów

> Używaj tego szablonu przy każdym commicie większej funkcji.

```md
### [RRRR‑MM‑DD] Tytuł/Temat
- Czego się nauczyłem/am:
- Link do podstrony / demka:
- Screenshot (opcjonalnie):
- Co poprawić następnym razem:
```

Przykład:

```md
### 2025‑08‑17 Flexbox – nawigacja responsywna
- align-items vs justify-content – kiedy co?
- Dodałem breakpointy na 480px/768px/1024px.
- TODO: dodać aria-current i focus styles dla linków.
```

---

## Mini–projekty

Pomysły na krótkie projekty (do 1–3h):

- **Glassmorphism Card** z hoverem 3D
- **Navbar Sticky** z cieniami i stanami focus
- **Form Validation** (HTML + JS, niestandardowe komunikaty)
- **Image Gallery** (grid, lazy‑loading, lightbox)
- **Todo App** (localStorage, filtry, edit‑in‑place)
- **Pogoda Mini** (fetch do publicznego API + fallback)

Każdy projekt powinien mieć:

- `README.md` (opis, funkcje, zrzuty ekranu),
- checklistę a11y i wydajności,
- notatkę *Czego się nauczyłem/am*.

---

## Zasady jakości

- **Semantyka:** poprawne tagi, nagłówki w kolejności, alt‑y dla obrazów.
- **Responsywność:** min. trzy progi, brak poziomego scrolla.
- **A11y:** focus widoczny, kontrast WCAG AA, aria‑\* tam gdzie trzeba.
- **Wydajność:** kompresja obrazów, `rel="preload"` kluczowych fontów, unikanie *layout thrashing*.
- **Kod:** spójne nazewnictwo (BEM), pliki < 500 linii na komponent, DRY.

**Checklist (kopiuj do projektu):**

```md
- [ ] Semantyka i nagłówki
- [ ] Responsywność (≤480 / 768 / ≥1024)
- [ ] Focus i aria‑labels
- [ ] Obrazy zoptymalizowane (format/rozmiar)
- [ ] Lighthouse: Performance ≥ 90, Accessibility ≥ 95
```

---

## Zadania / To‑Do

-

---

## Jak kontrybuować

Chcesz zasugerować poprawki lub pomysły? Super!

1. Zrób **fork** i nową gałąź z nazwą w stylu `feat/nazwa-funkcji`.
2. Opisz zmiany w PR: co, dlaczego, jak testować.
3. Dodaj zrzuty ekranu jeżeli to UI.

> Dla siebie: trzymaj *małe PR‑y* i częste commity z sensownymi wiadomościami.

---

## Licencja

Ten projekt (materiały edukacyjne i przykładowy kod) jest udostępniany na licencji **MIT**. Sprawdź plik `LICENSE` (jeśli brak — dodam wkrótce).

---

### Badges (opcjonalnie)

Dodaj pod tytułem, jeśli chcesz:

```md
![status](https://img.shields.io/badge/status-learning-blue)
![made-with](https://img.shields.io/badge/made%20with-HTML%2FCSS%2FJS-orange)
![license](https://img.shields.io/badge/license-MIT-green)
```

---

> Jeśli chcesz, mogę dostosować ten plik do faktycznej zawartości repo (nazwy folderów, zrzuty ekranu, link do GitHub Pages).

