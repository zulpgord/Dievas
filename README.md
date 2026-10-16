# Bestiario dell'Abisso

Diario per dare un nome alle proprie ansie e paure e trasformarle in creature: le colloca su una mappa dell'Inferno, ne segue l'andamento nel tempo e le libera in Paradiso quando smettono di comandare.

## Come è fatta

- L'app è tutta in `index.html`, senza build, server o dipendenze (solo i font Google, opzionali). Funziona anche aperta come file.
- `manifest.webmanifest`, `sw.js` e `icons/` la rendono installabile sul telefono e utilizzabile offline quando è servita dal sito (GitHub Pages: https://zulpgord.github.io/Dievas/).
- I dati restano nel browser (`localStorage`, chiave `bestiario.abisso.v1`). Nulla viene inviato in rete.
- Backup: dal Registro → *Custodia del tomo* si scarica un `.json` oppure il "tomo intero" (l'app con dentro i dati).

## Funzioni principali

- Creature con nome, dominio, trigger, sintomi e "che cosa faresti se non ci fosse".
- Voce rapida serale (potenza + terreno tenuto/ceduto) e rassegna serale.
- Sfide a gradini con paura prevista/reale e verifica della previsione.
- Modo notte (rimandare il rimuginio) e pagina "Se stai male adesso" con numeri di emergenza e ascolto.
- Termometro mensile GAD-7 (questionario standard, uso libero).
- Le funzioni si rivelano per gradi (3 voci → sfide, 10 voci → Registro completo); "Mostrare tutto subito" nel Registro.
- Promemoria serale come evento ricorrente nel calendario (.ics), con link `?rassegna=1`.
- Promemoria di backup dopo 7 giorni, condivisione del backup su telefono.

## Lingue

Italiano e inglese. Si cambia con il pulsante **EN / IT** in alto a destra; la scelta viene ricordata.

Nel codice ogni testo visibile è scritto come `L("italiano", "english")`: quando si aggiunge o modifica un testo, vanno scritte entrambe le versioni nello stesso punto.

## Usarla

Aprire `index.html` nel browser, oppure pubblicarla su qualsiasi hosting statico (GitHub Pages, Vercel, Netlify).
