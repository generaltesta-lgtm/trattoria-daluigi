# Trattoria da Luigi 🍝

Sito web dimostrativo per un ristorante, realizzato con **HTML, CSS e JavaScript**
puri (nessuna dipendenza).

## Struttura del progetto

```
test/
├── index.html          # Pagina principale
├── css/
│   └── style.css       # Stili
├── js/
│   └── main.js         # Interattività (menu mobile, form, scroll)
├── assets/
│   └── img/            # Immagini (hero.jpg, foto piatti, ecc.)
├── .gitignore
└── README.md
```

## Come provarlo in locale

Apri semplicemente `index.html` nel browser, oppure con un server locale:

```bash
# Python
python -m http.server 8000

# oppure Node
npx serve .
```

Poi vai su <http://localhost:8000>.

## Caricamento su GitHub (GitHub Pages)

1. Crea un nuovo repository su [github.com](https://github.com/new).
2. Da questa cartella:

   ```bash
   git init
   git add .
   git commit -m "Prima versione del sito del ristorante"
   git branch -M main
   git remote add origin https://github.com/<TUO-USER>/<REPO>.git
   git push -u origin main
   ```

3. Nel repository, vai su **Settings → Pages**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main`, cartella `/ (root)`
   - **Save**
4. Dopo qualche minuto il sito sarà online su:
   `https://<TUO-USER>.github.io/<REPO>/`

> I link e i path sono relativi, quindi il sito funziona anche sotto la
> sottocartella del repository (es. `/repo/index.html`).

## Personalizzazione

- **Nomi, piatti e prezzi**: modifica le sezioni in `index.html`.
- **Colori**: cambia le variabili in cima a `css/style.css` (blocco `:root`).
- **Immagini**: aggiungi foto in `assets/img/` (es. `hero.jpg`).
- **Contatti/form**: il form è una demo; per renderlo funzionante collega
  un servizio come [Formspree](https://formspree.io/) o il tuo backend.
