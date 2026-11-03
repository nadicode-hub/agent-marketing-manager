---
name: landing-page
description: Progetta e costruisce landing page e siti di una pagina belli e che convertono per una PMI italiana, a partire dal contesto e dal DESIGN.md dell'azienda. Struttura, testi, immagini, HTML e CSS responsive in un solo file, controllo visivo su telefono e computer, consegna pronta da pubblicare. Da usare per una landing page, una pagina di campagna, una pagina offerta, un mini sito, una pagina evento o il rifacimento di una pagina esistente.
license: Proprietary
metadata:
  hermes:
    tags: [Marketing, Landing page, Web design, HTML, Conversione]
    related_skills: [contesto-aziendale, metodo-marketing, direzione-artistica, design-md, claude-design, popular-web-designs, copywriting, cro, schema, marketing-italia]
---

# Landing page

Una landing page bella non basta: deve far fare una cosa sola, a una persona
precisa, su un telefono, in pochi secondi. Lavori come uno studio di design
bravo: prima il pensiero, poi la composizione, poi i dettagli.

## Prima di disegnare

1. Leggi `marketing/contesto.md` e `marketing/DESIGN.md`. Se manca il
   DESIGN.md, scrivilo prima con `direzione-artistica`.
2. Scrivi il brief con `metodo-marketing`: per chi, da dove arriva (annuncio,
   Google, QR del volantino, Instagram), idea dominante, **una** azione
   principale.
3. Per processo e gusto segui la skill `claude-design`; se il titolare vuole
   lo stile di un sito famoso, usa `popular-web-designs` come vocabolario,
   sempre piegato ai colori e ai caratteri del DESIGN.md.

## La struttura che funziona per una PMI

Adatta, togli quello che non serve, non aggiungere sezioni per riempire:

1. **In alto, senza scorrere:** cosa offri e a chi in un titolo concreto,
   una riga che toglie il dubbio principale, il pulsante dell'azione (Chiama,
   Scrivici su WhatsApp, Prenota, Chiedi un preventivo) e un'immagine vera.
2. **Prova subito sotto:** valutazione e numero di recensioni Google, loghi di
   clienti che si possono citare, anni di attività, un numero vero.
3. **Cosa ottieni:** tre o quattro benefici concreti, nelle parole del
   cliente.
4. **Come funziona:** tre passi, dal contatto al risultato.
5. **L'offerta:** cosa è incluso, prezzo o "da", condizioni, scadenza vera se
   c'è (sconti con il prezzo più basso a 30 giorni, vedi `marketing-italia`).
6. **Recensioni o casi:** testi veri, con nome e permesso.
7. **Domande frequenti:** le obiezioni reali (prezzo, tempi, zona, garanzia).
8. **Di nuovo l'azione,** con orari e zona servita, mappa se c'è una sede.
9. **Piè di pagina:** ragione sociale, indirizzo, partita IVA, contatti,
   privacy e cookie.

Su mobile il pulsante principale resta raggiungibile (barra fissa in basso con
Chiama e WhatsApp per le attività locali). Moduli brevi: nome, telefono o
email, una domanda, consenso privacy separato e non preselezionato.

## Costruire

- Un solo file `index.html` con CSS nel file, nella cartella
  `marketing/pagine/<nome>/`, immagini accanto in formato WebP. Niente
  framework se non servono.
- I token del DESIGN.md diventano variabili CSS (`--colore-primario`,
  `--font-titoli`...). Caratteri da Google Fonts, al massimo due famiglie.
- Responsive da 360 px a 1440 px, testo base almeno 16 px, contrasto almeno
  4,5:1, pulsanti alti almeno 44 px, immagini con `alt` in italiano, titoli
  in ordine (un solo `h1`).
- Link diretti: `tel:+39...`, `https://wa.me/39...?text=...` con un messaggio
  precompilato, `mailto:`.
- Metatag: titolo e descrizione per Google, immagine per la condivisione
  (Open Graph), e i dati strutturati dell'attività con la skill `schema`.
- Veloce: immagini dimensionate, nessuno script inutile, niente slider
  automatici.
- Nessun cookie di profilazione o pixel finché non c'è un banner di consenso
  conforme.

## Guardarla prima di mostrarla

Apri la pagina nel tuo browser e guardala tutta, a 390 px e a 1440 px di
larghezza. Correggi prima di mostrarla:

- testo che va a capo male, titoli troppo lunghi su mobile;
- spazi irregolari, elementi non allineati, immagini tagliate o sgranate;
- colori fuori dal DESIGN.md, contrasto basso;
- pulsante principale non visibile senza scorrere;
- link telefono e WhatsApp sbagliati;
- l'aria da modello generico: se togliendo il logo potrebbe essere di
  chiunque, manca qualcosa di vero dell'azienda.

Poi mostra al titolare la pagina vera (il file HTML), con due righe: per chi è
e quale azione chiede. Proponi una variante solo se cambia davvero qualcosa
(un'altra idea dominante, un'altra struttura), non un colore diverso.

## Pubblicare

Pubblicare richiede il sì del titolare. Consegna la cartella pronta e, se il
titolare ti dà l'accesso al suo hosting o al suo costruttore di siti
(WordPress, Wix, Shopify, Netlify, Cloudflare Pages...), pubblicala tu
seguendo le istruzioni di quel servizio, poi verifica l'indirizzo pubblico su
telefono e computer.
