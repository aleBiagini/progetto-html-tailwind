# Url sito produzione
https://progetto-html-tailwind.netlify.app/
# Nome Progetto

Progetto html + tailwind!

---

## Cos’è

Questo repository contiene il codice sorgente del progetto, una pagina pubblicata automaticamente su **Netlify**.  
Caratteristiche principali:

* **Stack**: (HTML Tailwind CSS)  
* **Deploy continuo**: ogni push su `main` o su una branch di feature crea un deploy preview su Netlify.  
* **CI integrata**: build, test e ottimizzazione avvengono dentro la pipeline Netlify.  

---

## Come lavorarci

> Segui il diagramma sottostante per capire il ciclo di sviluppo completo — dal clone alla pubblicazione.

```mermaid
flowchart TD
    A[Clona il repository<br/>git clone …] --> B[Installa le dipendenze<br/>npm ci]
    B --> C[Avvia ambiente locale<br/>npm run dev]
    C --> D[Modifica il codice<br/> feature / fix ]
    D --> E[Commit & push<br/>git add . && git commit && git push]
    E --> F[Build automatica su Netlify]
    F --> G[Deploy preview o produzione<br/>URL *.netlify.app]
