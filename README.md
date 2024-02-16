# Modulo React Post Viewer
Il modulo "React Post Viewer" è stato progettato per semplificare la visualizzazione di tutti i post di Joomla direttamente nel frontend. Sfruttando la potenza di React e Vite JS, questo modulo offre una soluzione moderna e reattiva per presentare in modo accattivante e user-friendly i contenuti del tuo sito Joomla.

<div align="center">
  <a href="https://github.com/joomla/joomla-cms" target="_blank" rel="noopener noreferrer">
    <img src="https://www.joomla.it/images/immagini/sampledata/Joomla-flat-logo-en.png" alt="Logo Joomla" width="100" height="100">
  </a>
  <a href="https://github.com/vitejs/vite" target="_blank" rel="noopener noreferrer">
    <img src="https://vitejs.dev/logo.svg" alt="Logo Vite JS" width="100" height="100">
  </a>
  <a href="https://it.legacy.reactjs.org/" target="_blank" rel="noopener noreferrer">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/768px-React-icon.svg.png" alt="Logo React" width="100">
  </a>
</div>

## Descrizione
Joomla è un robusto sistema di gestione dei contenuti, e con questo modulo React JS, hai la possibilità di portare la tua esperienza utente al livello successivo.

Questo progetto fornisce un'interfaccia semplificata per la compilazione automatica di React all'interno di Joomla 4, grazie all'integrazione di Vite JS. Vite JS, con la sua architettura basata su ESM (ECMAScript Modules), offre una compilazione veloce e una gestione efficiente delle dipendenze, rendendo il processo di sviluppo più fluido ed efficiente.

## Caratteristiche Principali
* **Visualizzazione di tutti i Post**: Il modulo consente agli utenti di visualizzare una lista completa di tutti i post presenti sul tuo sito Joomla direttamente dalla pagina frontend.
* **Interfaccia Utente Reattiva**: Sfruttando la potenza di React JS e la velocità di Vite JS, il modulo offre un'interfaccia utente reattiva che si adatta perfettamente a diverse dimensioni di schermo e dispositivi.
* **Compilazione Veloce con Vite JS**: Grazie a Vite JS, il processo di compilazione del tuo progetto React è rapido ed efficiente, migliorando notevolmente i tempi di sviluppo.

## Prerequisiti
Prima di utilizzare questo progetto, assicurati di soddisfare i seguenti prerequisiti:

> [!WARNING]
> * **Joomla 4**: Verifica di utilizzare la versione raccomandata di PHP 8.2.
> * **Vite JS**: Assicurati di avere installata una versione di Node.js pari a 18.0.0 o superiore, ma inferiore a 20.0.0.

## Come Iniziare
Segui le istruzioni nel README per installare e configurare React con Vite JS all'interno del tuo progetto Joomla. Inizia a sfruttare i vantaggi di una compilazione veloce e di un flusso di lavoro ottimizzato per lo sviluppo frontend.

### Installazione e Configurazione di Joomla
1. **Scarica Joomla:**
Visita [la pagina di download di Joomla](https://downloads.joomla.org/it/latest) e scarica l'ultima versione del CMS Joomla.

2. **Estrai i File:**
Dopo aver scaricato il file zip, estrailo nella directory del tuo server web. Puoi utilizzare strumenti come WinZip o un'utility di estrazione integrata.

3. **Database MySQL:**
Assicurati di avere un database MySQL pronto per essere utilizzato. Crea un nuovo database e un utente associato attraverso il tuo strumento di gestione del database (ad esempio, phpMyAdmin).

4. **Configurazione File `configuration.php`:**
Rinomina il file `configuration.php-dist` nella directory principale di Joomla in `configuration.php`. Modifica questo file con le informazioni del tuo database e altre configurazioni necessarie.

5. **Installazione da Browser:**
Accedi al tuo sito Joomla attraverso un browser. Segui la procedura di installazione guidata. Sarai guidato attraverso la configurazione della lingua, la connessione al database e la configurazione del sito.

6. **Configurazione Amministratore:**
Durante l'installazione, verrà richiesto di configurare l'account amministratore principale. Fornisci le informazioni richieste, inclusa l'email e la password.

7. **Rimozione Installazione:**
Dopo aver completato la procedura di installazione, assicurati di rimuovere la cartella installation dal tuo server per motivi di sicurezza.

8. **Accesso al Pannello di Controllo:**
Accedi al pannello di controllo amministrativo di Joomla utilizzando le credenziali dell'account amministratore.

### Creazione del File `package.json`

1. **Apri un Terminale:**
Assicurati di trovarati nella directory principale del tuo progetto Joomla.

2. **Crea il File `package.json`:**
Utilizza il tuo editor di testo preferito o il comando touch per creare il file `package.json` nella directory principale del tuo progetto. Incolla al suo interno il seguente codice:

```json
{
    "name": "joomla",
    "version": "5.0.2",
    "description": "Joomla CMS",
    "license": "GPL-2.0-or-later",
    "dependencies": {
        "react": "^18.2.0",
        "react-dom": "^18.2.0"
    },
    "devDependencies": {
        "@types/react": "^18.2.43",
        "@types/react-dom": "^18.2.17",
        "@vitejs/plugin-react": "^4.2.1",
        "eslint": "^8.55.0",
        "eslint-plugin-react": "^7.33.2",
        "eslint-plugin-react-hooks": "^4.6.0",
        "eslint-plugin-react-refresh": "^0.4.5",
        "sass": "^1.69.5",
        "vite": "^5.0.8"
    }
}
```

### Esecuzione del Comando `npm install`
1. **Apri un Terminale:**
Assicurati di essere ancora nella directory principale del tuo progetto Joomla.

2. **Esegui il Comando `npm install`:**
Digita il seguente comando e premi Invio per eseguire l'installazione delle dipendenze elencate nel file `package.json`:

```bash
npm install
```
Questo comando installerà le dipendenze necessarie, inclusi React, Sass e Vite, nel tuo progetto.

3. **Attendi il Completamento:**
L'installazione richiederà qualche istante. Attendi pazientemente finché il processo non è completato.