# 📋 Registro Presenze Tirocinanti

PWA self-contained per la gestione delle presenze in negozio.
Funziona offline, installabile come app su Android e iOS.

---

## 🚀 Pubblicare su GitHub Pages (3 minuti)

### Passo 1 — Crea il repository
1. Vai su [github.com](https://github.com) → clic su **"New"**
2. Nome repository: `presenze-tirocinanti`
3. Visibilità: ✅ **Public**
4. Clic **"Create repository"**

### Passo 2 — Carica i file
Nella pagina del repository appena creato:
1. Clic su **"uploading an existing file"** (o "Add file" → "Upload files")
2. Trascina dentro questi 3 file: `index.html`, `manifest.json`, `sw.js`
3. Clic **"Commit changes"**

### Passo 3 — Attiva GitHub Pages
1. Vai in **Settings** (in alto nel repository)
2. Sezione sinistra → clic **"Pages"**
3. Under "Source" → seleziona **"Deploy from a branch"**
4. Branch: **main** | Folder: **/ (root)**
5. Clic **"Save"**

⏳ Dopo 1-2 minuti l'app sarà online su:
```
https://TUO-USERNAME.github.io/presenze-tirocinanti/
```

---

## 📱 Convertire in APK con PWABuilder (gratis, no codice)

1. Vai su **[pwabuilder.com](https://www.pwabuilder.com)**
2. Incolla il tuo URL GitHub Pages
3. Clic **"Start"** → aspetta l'analisi (30 sec)
4. Clic **"Package for stores"**
5. Scegli **Android** → **Generate Package**
6. Scarica lo zip → estrai → trovi l'APK

### Installare l'APK su Android
1. Trasferisci l'APK sul telefono (via cavo o email)
2. Apri il file → se chiesto, abilita "Installa da sorgenti sconosciute"
3. Clic "Installa" → l'app appare nella home

---

## ℹ️ Note tecniche
- Tutti i dati sono salvati localmente sul dispositivo (localStorage)
- Funziona offline dopo il primo caricamento
- Le icone sono embedded nel manifest (nessun file extra necessario)
