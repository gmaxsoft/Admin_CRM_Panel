# Data Fox – Tailwind Admin Template

Panel administracyjny oparty na Tailwind CSS z obsługą trybu ciemnego i responsywnym układem.

## Stack technologiczny

### Frontend
| Technologia | Wersja | Opis |
|-------------|--------|------|
| **Tailwind CSS** | ^3.4.19 | Framework utility-first do stylowania |
| **Sass** | ^1.97.3 | Preprocesor CSS |
| **PostCSS** | (via gulp-postcss) | Przetwarzanie CSS (Tailwind, Autoprefixer) |
| **Animate.css** | ^4.1.1 | Animacje CSS |
| **Feather Icons** | ^4.29.2 | Zestaw ikon SVG |
| **SimpleBar** | ^6.3.3 | Niestandardowe paski przewijania |
| **WOW.js** | ^1.2.2 | Animacje przy przewijaniu |
| **Clipboard.js** | ^2.0.11 | Kopiowanie do schowka |
| **Popper.js** | ^2.11.8 | Pozycjonowanie dropdownów i tooltipów |

### Build & Dev Tools
| Technologia | Wersja | Opis |
|-------------|--------|------|
| **Gulp** | ^4.0.2 | Automatyzacja zadań |
| **Babel** | ^7.29.0 | Transpilacja JavaScript (ES6+) |
| **Browser-Sync** | ^3.0.2 | Serwer deweloperski z live reload |
| **Prettier** | ^3.8.1 | Formatowanie kodu |
| **gulp-sass** | ^5.1.0 | Kompilacja SCSS |
| **gulp-postcss** | ^10.0.0 | Integracja PostCSS z Gulp |
| **gulp-file-include** | ^2.3.0 | Szablony HTML (include) |
| **gulp-htmlmin** | ^5.0.1 | Minifikacja HTML |
| **gulp-uglify** | ^3.0.2 | Minifikacja JavaScript |
| **gulp-autoprefixer** | ^6.1.0 | Automatyczne prefiksy CSS |
| **gulp-imagemin** | ^9.0.0 | Optymalizacja obrazów |

### Konfiguracja
- **Node.js** – środowisko uruchomieniowe
- **npm** – menedżer pakietów

## Instalacja

```bash
npm install
```

## Skrypty

| Polecenie | Opis |
|-----------|------|
| `npm start` | Uruchamia serwer deweloperski (Browser-Sync) i otwiera `/dashboard/` |
| `npm run build` | Buduje projekt produkcyjny do folderu `dist/` |
| `npm run format` | Formatuje kod w `./src` za pomocą Prettier |

## Struktura projektu

```
├── src/
│   ├── html/           # Szablony HTML
│   │   ├── dashboard/  # Strona główna panelu
│   │   ├── layouts/    # Layouty, header, sidebar, footer
│   │   ├── pages/      # Login, rejestracja
│   │   └── elements/   # Komponenty UI
│   ├── assets/
│   │   ├── scss/       # Style SCSS
│   │   ├── js/         # Skrypty JavaScript
│   │   ├── images/     # Obrazy
│   │   └── fonts/      # Czcionki, ikony
│   └── ...
├── tailwind_plugins/   # Własne pluginy Tailwind
├── dist/               # Zbudowana wersja produkcyjna
├── gulpfile.js         # Konfiguracja Gulp
├── tailwind.config.js  # Konfiguracja Tailwind
└── postcss.config.js   # Konfiguracja PostCSS
```

## Funkcje

- Tryb ciemny (domyślny) i jasny
- Responsywny układ (vertical, horizontal, compact, tab)
- Różne motywy kolorystyczne (preset-1 do preset-10)
- Obsługa RTL
- Ikony: Feather, Tabler, Phosphor, Font Awesome, Material
