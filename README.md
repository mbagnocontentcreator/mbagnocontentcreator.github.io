# MB Apps - Sito Vetrina

Sito web vetrina per le app sviluppate da Matteo Bagno.

**URL Live:** https://mbagnocontentcreator.github.io

---

## Struttura del Progetto

```
mbb-apps-site/
├── index.html                    # Homepage principale
├── logo.png                      # Logo MB (tema scuro, sfondo trasparente)
├── logo-dark-theme.png           # Copia backup del logo tema scuro
├── LOGO.jpg                      # Logo originale (colori verde/arancione)
├── portfolio-tracking-icon.png   # Icona app Portfolio Tracking
├── portfolio-tracking/
│   ├── privacy.html              # Privacy Policy
│   └── support.html              # Pagina Supporto e FAQ
└── README.md                     # Questo file
```

---

## App Pubblicate

### 1. Portfolio Tracking
- **Piattaforma:** iPad
- **App Store:** https://apps.apple.com/it/app/portfolio-tracking/id6756198088
- **Descrizione:** App per monitorare e analizzare le performance degli investimenti
- **Data pubblicazione sito:** 10 Dicembre 2025

---

## Come Aggiungere una Nuova App

1. **Crea la cartella dell'app** (es. `nuova-app/`)
   - Aggiungi `privacy.html`
   - Aggiungi `support.html`

2. **Aggiungi l'icona** nella root (es. `nuova-app-icon.png`)

3. **Modifica `index.html`** - Aggiungi una nuova card nella sezione `apps-grid`:

```html
<div class="app-card">
    <div class="app-header">
        <img src="nuova-app-icon.png" alt="Nome App" class="app-icon">
        <div>
            <h2 class="app-title">Nome App</h2>
            <p class="app-tagline">Tagline dell'app</p>
        </div>
    </div>

    <div class="platform-badge">
        <svg viewBox="0 0 24 24" fill="currentColor"><rect x="4" y="2" width="16" height="20" rx="2" ry="2" fill="none" stroke="currentColor" stroke-width="2"/><line x1="12" y1="18" x2="12" y2="18" stroke="currentColor" stroke-width="2" stroke-linecap="round"/></svg>
        Disponibile su iPad
    </div>

    <p class="app-description">Descrizione dell'app...</p>

    <a href="URL_APP_STORE" class="app-store-btn" target="_blank" rel="noopener">
        <svg viewBox="0 0 24 24" fill="currentColor">
            <path d="M18.71 19.5c-.83 1.24-1.71 2.45-3.05 2.47-1.34.03-1.77-.79-3.29-.79-1.53 0-2 .77-3.27.82-1.31.05-2.3-1.32-3.14-2.53C4.25 17 2.94 12.45 4.7 9.39c.87-1.52 2.43-2.48 4.12-2.51 1.28-.02 2.5.87 3.29.87.78 0 2.26-1.07 3.81-.91.65.03 2.47.26 3.64 1.98-.09.06-2.17 1.28-2.15 3.81.03 3.02 2.65 4.03 2.68 4.04-.03.07-.42 1.44-1.38 2.83M13 3.5c.73-.83 1.94-1.46 2.94-1.5.13 1.17-.34 2.35-1.04 3.19-.69.85-1.83 1.51-2.95 1.42-.15-1.15.41-2.35 1.05-3.11z"/>
        </svg>
        <span>
            <span class="small-text">Scarica su</span>
            <span class="big-text">App Store</span>
        </span>
    </a>

    <div class="app-links">
        <a href="nuova-app/privacy.html">Privacy Policy</a>
        <a href="nuova-app/support.html">Supporto</a>
    </div>
</div>
```

4. **Commit e push:**
```bash
git add .
git commit -m "Add [Nome App] to showcase"
git push
```

---

## Badge Piattaforma

Per **iPhone** usa:
```html
<div class="platform-badge">
    <svg viewBox="0 0 24 24" fill="currentColor"><rect x="6" y="2" width="12" height="20" rx="2" ry="2" fill="none" stroke="currentColor" stroke-width="2"/><line x1="12" y1="18" x2="12" y2="18" stroke="currentColor" stroke-width="2" stroke-linecap="round"/></svg>
    Disponibile su iPhone
</div>
```

Per **iPhone e iPad** usa:
```html
<div class="platform-badge">
    <svg>...</svg>
    Disponibile su iPhone e iPad
</div>
```

---

## Cronologia Modifiche

| Data | Descrizione |
|------|-------------|
| 10/12/2025 | Redesign completo: layout griglia, logo MB tema scuro, pulsante App Store, badge piattaforma |
| 06/12/2025 | Aggiornato email contatto a info@matteobagno.com |
| 06/12/2025 | Commit iniziale con Privacy Policy e Supporto per Portfolio Tracking |

---

## Contatti

- **Email:** info@matteobagno.com
- **GitHub:** https://github.com/mbagnocontentcreator
