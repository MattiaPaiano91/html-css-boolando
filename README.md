Vite Yu-Gi-Oh
Questo progetto è un'applicazione web sviluppata con Vue 3 e Vite, che utilizza l'API di Yu-Gi-Oh (https://db.ygoprodeck.com/api/v7/cardinfo.php) per visualizzare una griglia di carte Yu-Gi-Oh.

Descrizione
L'applicazione è strutturata secondo il layout mostrato nello screenshot fornito. Al caricamento della pagina, viene effettuata una chiamata AJAX all'API di Yu-Gi-Oh per recuperare i dati delle carte. Per evitare rallentamenti o attese eccessivi, la richiesta utilizza i parametri num e offset per limitare il numero di risultati restituiti.

Le carte recuperate vengono visualizzate in una griglia, con un componente Card personalizzato per ogni carta. Durante il caricamento dei dati, viene mostrato un componente Loader per segnalare all'utente che i dati sono in fase di recupero.

Tecnologie utilizzate
Vue 3
Vite
Axios (o altra libreria per le chiamate AJAX)
Installazione
Clonare il repository
Eseguire npm install per installare le dipendenze
Eseguire npm run dev per avviare l'applicazione in modalità di sviluppo
Aprire http://localhost:3000 (o l'URL specificato dal server di sviluppo) nel browser
Struttura del progetto
src/App.vue: Componente principale dell'applicazione
src/components/Card.vue: Componente che rappresenta una singola carta Yu-Gi-Oh
src/components/Loader.vue: Componente che visualizza un'animazione di caricamento
src/services/api.js: Modulo che contiene le funzioni per effettuare le chiamate AJAX all'API di Yu-Gi-Oh
Documentazione
La documentazione dell'API di Yu-Gi-Oh è disponibile all'indirizzo: https://ygoprodeck.com/api-guide/
