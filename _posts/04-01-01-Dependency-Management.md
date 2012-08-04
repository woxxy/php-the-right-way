# Gestione delle Dipendenze

Esiste una tonnellata di librerie PHP, framework e componenti dai quali scegliere. Il tuo progetto probabilmente userà molti di questi - questi sono dipendenze del progetto. Fino a recente data PHP non aveva alcun buon metodo per gestire le dipendenze dei progetti. Anche se le gestissi manualmente, avresti dovuto comunque preoccuparti degli autoloader. Non più.

Correntemente ci sono due maggiori sistemi di gestione dei pacchetti per PHP - Composer e PEAR. Quale è adatto a te? La risposta è entrambi.

 * Usa **Composer** per gestire le dipendenze per un singolo progetto.
 * Use **PEAR** per gestire le dipendenze di PHP in generale per il tuo sistema.
 
In generale, i pacchetti di Composer saranno disponibili solo nei progetti in cui li specifichi esplicitamente, mentre i pacchetti PEAR saranno disponibili per tutti i tuoi progetti PHP. Mentre a prima vista PEAR può apparire come un approccio più semplice, ci sono vantaggi ad utilizzare un approccio per-progetto delle tue dipendenze.