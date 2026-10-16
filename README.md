# Bestiario dell'Abisso

Diario per dare un nome alle proprie ansie e paure e trasformarle in creature: le colloca su una mappa dell'Inferno, ne segue l'andamento nel tempo e le libera in Paradiso quando smettono di comandare.

## Come è fatta

- Un solo file: `index.html`, senza build, server o dipendenze (solo i font Google, opzionali).
- I dati restano nel browser (`localStorage`, chiave `bestiario.abisso.v1`). Nulla viene inviato in rete.
- Backup: dal Registro → *Custodia del tomo* si scarica un `.json` oppure il "tomo intero" (l'app con dentro i dati).

## Lingue

Italiano e inglese. Si cambia con il pulsante **EN / IT** in alto a destra; la scelta viene ricordata.

Nel codice ogni testo visibile è scritto come `L("italiano", "english")`: quando si aggiunge o modifica un testo, vanno scritte entrambe le versioni nello stesso punto.

## Usarla

Aprire `index.html` nel browser, oppure pubblicarla su qualsiasi hosting statico (GitHub Pages, Vercel, Netlify).
