# 🍿 Carretto UCI - Web App Cassa

Questa è una **Progressive Web App (PWA)** leggera e veloce creata per gestire le vendite e i calcoli di cassa in mobilità.
È stata progettata specificamente con uno stile iOS nativo per offrire un'esperienza fluida e intuitiva su iPhone.

## 🚀 Funzionalità Principali

- **Griglia Prodotti**: Selezione rapida dei prodotti UCI con prezzi preimpostati.
- **Calcolo Totale**: Somma automatica del carrello in tempo reale.
- **Gestione Pagamenti**: 
  - Pulsante dedicato per pagamenti con Carta.
  - Sezione Contanti con tagli rapidi (€2, €5, €10, €20, €50).
  - Calcolo automatico del resto.
- **Report Giornaliero**: Monitoraggio degli incassi (divisi per Carta e Contanti) e conteggio dei pezzi venduti per ogni singolo prodotto.
- **Feedback Aptico (Vibrazione)**: Supporto per la vibrazione di sistema alla pressione dei tasti (ottimizzato per iOS 18+).
- **Design Nativo**: Interfaccia in Dark Mode che ricalca lo stile "Inset Grouped" delle impostazioni iOS.
- **Offline & Privacy**: Tutti i dati sono salvati localmente sul dispositivo (localStorage) e non vengono inviati ad alcun server esterno.

## 📱 Installazione su iPhone (PWA)

Non è necessario scaricare l'app dall'App Store. Essendo una PWA, puoi installarla direttamente da Safari:

1. Apri il link del sito su **Safari**.
2. Tocca l'icona **Condividi** (il quadrato con la freccia verso l'alto).
3. Scorri le opzioni e seleziona **"Aggiungi alla schermata Home"**.
4. Conferma cliccando su **"Aggiungi"**.

L'app apparirà ora sulla tua Home con la sua icona e funzionerà a tutto schermo, proprio come un'app nativa.

## 🛠 Note Tecniche

- **Linguaggi**: HTML5, CSS3 (Flexbox/Grid), JavaScript (Vanilla).
- **Storage**: Utilizza `localStorage` per la persistenza dei dati del report.
- **Haptic Feedback**: Implementato tramite il trucco `switch` per la compatibilità con le restrizioni di Safari su iOS 18.
- **Responsività**: Ottimizzata per schermi iPhone (testata su iPhone 13/14/15/16).

## 📋 Manutenzione e Modifiche

### Cambiare i prezzi o i prodotti
Per aggiornare l'elenco dei prodotti o i prezzi, è sufficiente modificare la costante `prodotti` nel file `index.html`:

```javascript
const prodotti = [
    {nome: "Pop Corn Salati", prezzo: 5.60},
    // Aggiungi o modifica qui...
];
```

## 📋 Reset dei dati
Il tasto "AZZERA REPORT GIORNALIERO" nel foglio Report pulisce tutte le statistiche accumulate.
Per una pulizia profonda dell'app, è necessario svuotare la cache del browser o rimuovere l'app dalla Home e reinstallarla.

---

*Sviluppato con passione per ottimizzare il lavoro di squadra.*
