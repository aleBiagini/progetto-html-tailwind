# Nome Progetto

Breve slogan del progetto (es. “Un sito personale in Astro distribuito su Netlify”).  
Modifica questo paragrafo con uno‐due frasi che spieghino **perché** esiste e **che problema risolve**.

---

## Cos’è

Questo repository contiene il codice sorgente di **Nome Progetto**, un’applicazione front-end renderizzata lato build e pubblicata automaticamente su **Netlify**.  
Caratteristiche principali:

* **Framework**: (es. Astro + Tailwind CSS)  
* **Deploy continuo**: ogni push su `main` o su una branch di feature crea un deploy preview su Netlify.  
* **CI integrata**: build, test e ottimizzazione avvengono dentro la pipeline Netlify.  
* **Zero config**: tutto è definito in `package.json` e facoltativamente in `netlify.toml`.

Sostituisci (o rimuovi) i punti che non si applicano al tuo stack.

---

## Come lavorarci

> Segui il diagramma sottostante per capire il ciclo di sviluppo completo — dal clone alla pubblicazione.

```mermaid
flowchart TD
    A[Clona il repository<br/>git clone …] --> B[Installa le dipendenze<br/>npm ci]
    B --> C[Avvia ambiente locale<br/>npm run dev]
    C --> D[Modifica il codice<br/>(feature / fix)]
    D --> E[Commit & push<br/>git add . && git commit && git push]
    E --> F[Build automatica su Netlify]
    F --> G[Deploy preview o produzione<br/>URL *.netlify.app]
