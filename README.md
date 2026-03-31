# 📋 Registro Presenze Tirocinanti

PWA per la gestione delle presenze dei tirocinanti in negozio.

## 🚀 Deploy su GitHub Pages

### 1. Crea il repository
1. Vai su [github.com](https://github.com) → **New repository**
2. Nome: `presenze-tirocinanti`
3. Visibilità: **Public** (necessario per GitHub Pages gratuito)
4. Clicca **Create repository**

### 2. Carica i file
```bash
git clone https://github.com/TUO-USERNAME/presenze-tirocinanti.git
cd presenze-tirocinanti
# copia qui: index.html, manifest.json, sw.js, icons/
git add .
git commit -m "Prima versione PWA presenze"
git push origin main
```

### 3. Attiva GitHub Pages
1. Repository → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` → `/ (root)`
4. Clicca **Save**
5. Dopo ~2 minuti la PWA sarà su: `https://TUO-USERNAME.github.io/presenze-tirocinanti/`

---

## 📱 Conversione in APK (metodo consigliato: PWABuilder)

### Metodo A — PWABuilder (più semplice, nessuna installazione)

1. Vai su **[pwabuilder.com](https://www.pwabuilder.com)**
2. Incolla l'URL: `https://TUO-USERNAME.github.io/presenze-tirocinanti/`
3. Clicca **Start** → attendi l'analisi
4. Clicca **Package for stores** → scegli **Android**
5. Scarica il pacchetto `.apk` o `.aab`
6. Installa l'APK sul telefono (abilita "Sorgenti sconosciute" nelle impostazioni Android)

### Metodo B — Bubblewrap CLI (più controllo)

#### Prerequisiti
- Node.js 14+
- Java JDK 8+
- Android SDK

```bash
# Installa Bubblewrap
npm install -g @bubblewrap/cli

# Inizializza il progetto TWA
bubblewrap init --manifest https://TUO-USERNAME.github.io/presenze-tirocinanti/manifest.json

# Compila l'APK
bubblewrap build

# L'APK sarà in: ./app/build/outputs/apk/release/app-release-signed.apk
```

---

## 📂 Struttura file

```
presenze-tirocinanti/
├── index.html          # App principale
├── manifest.json       # Config PWA
├── sw.js               # Service Worker (offline)
├── icons/
│   ├── icon-192.png    # Icona app
│   └── icon-512.png    # Icona splash screen
└── README.md
```

---

## ✅ Checklist prima della conversione APK

- [ ] GitHub Pages attivo e raggiungibile via HTTPS
- [ ] `manifest.json` con `start_url`, `icons` (192x192 e 512x512)
- [ ] Service Worker registrato correttamente
- [ ] App testata su mobile dal browser
