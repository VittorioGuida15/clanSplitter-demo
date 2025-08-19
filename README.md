# 🏰 ClanSplitter per Clash of Clans (Demo)

ClanSplitter è una piccola applicazione web, legata al mondo del videogioco Clash of Clans, pensata per aiutare il capo e co-capi a organizzare la CWL (Lega delle Guerre tra Clan): recupera i membri di un clan principale, li ordina per TH e ti permette di suddividerli rapidamente in più clan, generando messaggi pronti da condividere.

Attualmente deployata al seguente URL: https://clansplitter.netlify.app/

L'applicazione è costruita con un'architettura moderna ibrida:
   -   **Frontend:** *React (Vite)* e ospitata su *Netlify*.
   -   **Backend:** *Node.js (Express)* e ospitato su *Render* per ottenere IP statici necessari alle API di Clash of Clans.

## ⚡️ Funzionalità

   -   **Configurazione Dinamica dei Clan:** Aggiungi, modifica e rimuovi un numero qualsiasi di clan di destinazione.
   -   **Caricamento Automatico dei Dati:** Inserendo il tag di un clan, l'app recupera automaticamente il nome, la lega e genera il link di invito.
   -   **Recupero Membri del Clan Principale:** Carica e visualizza la lista completa dei membri del tuo clan, ordinata per livello del Municipio (TH).
   -   **Assegnazione Semplificata:** Con un semplice clic, assegna ogni giocatore a uno dei clan di destinazione.
   -   **Generazione Automatica di Messaggi:** Crea messaggi di testo formattati per ogni clan, con la lista dei giocatori assegnati, pronti per essere copiati.
   -   **Salvataggio Locale:** Tutte le configurazioni dei clan vengono salvate nel browser, quindi non è necessario reinserirle a ogni avvio.

⚠️ Limitazioni. **Cold start (Render free):** *La prima chiamata dopo un periodo di inattività può essere lenta; le successive sono rapide.*

## 🎬 Demo Video
<video src="risorse/demo.mp4" controls width="100%"></video>

## 📁 Struttura del progetto

```
clanSplitter-serverized/
├── public/                 
│   └── vite.svg            → Logo app default
│          
├── server/                 
│   ├── package-lock.json   → Versioni delle dipendenze
│   ├── package.json        → Dipendenze per il server
│   └── server.js           → Codice del server (back-end) che comunica con L'API di Clash of Clans
│
├── src/                    
│   ├── App.css             → CSS per App.jsx
│   ├── App.jsx             → Componente React principale (front-end)
│   ├── assets/             → Eventuali immagini
│   ├── index.css           → Stili CSS globali
│   └── main.jsx            → Punto di ingresso per il codice lato client
│
├── .gitignore              → File e cartelle da ignorare per Git
├── .eslintrc.cjs           → Configurazione di ESLint
├── index.html              → Pagina HTML principale
├── netlify.toml            → Configurazione per il deploy su Netlify
├── package-lock.json       → Versioni delle dipendenze del progetto
├── package.json            → Dipendenze del progetto
├── README.md               → Documentazione del progetto
└── vite.config.js          → Configurazione per Vite
```

### 👷🏻‍♂️ Autore: Vittorio Guida


