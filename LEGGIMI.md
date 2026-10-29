# Bolzano Express — guida ibrida (GitHub Pages + foglio Google)

## Cosa c'è
- `index.html`: la guida (un solo file). `mappa.jpg`: la mappa satellitare della presentazione. `foto/`: foto delle prove, suggerimenti e arrivo.
- `foglio-guida.csv`: i 21 contenuti importati dalla presentazione. Importalo in Google Sheets (File → Importa) come nuova scheda, per esempio `Guida_Eventi`.

## Pubblicare
1. Crea un repository GitHub e carica tutto il contenuto della cartella.
2. Settings → Pages → Branch `main`, cartella `/ (root)`.
3. Il link sarà `https://tuonome.github.io/nome-repo/`.

## Collegare il foglio
1. Nel foglio: File → Condividi → Pubblica sul web → scegli **solo** la scheda Guida_Eventi → formato CSV.
2. Incolla il link in `CONFIG.foglioCSV` dentro `index.html`. Senza link la guida usa i dati incorporati.
3. Le modifiche al foglio compaiono entro qualche minuto.

## Colonne del foglio
`id, titolo, categoria, x, y, lx, ly, punti, testo, foto, aiuto, link, visibile`
- categoria: `obbligatoria` (rosso), `localizzata` (oro), `libera` (blu petrolio).
- x, y: dove punta la linea sulla mappa (% della mappa, 0–100). Vuote per le prove non localizzate.
- lx, ly: dove sta il cartiglio (% della mappa). Le prove libere hanno solo questi.
- foto: nome del file in `foto/`. aiuto: immagini di suggerimento separate da virgola. link: pulsante opzionale (es. il brano del Teatro). visibile: `1` o `0`.

## Altra città
Sostituisci `mappa.jpg` (16:9) e `foto/`, cambia `CONFIG` (titolo, arrivo, WhatsApp, regolamento, riquadro) e riposiziona x, y, lx, ly nel foglio.

## Da controllare
- Punti: Mercato della frutta è 10–90 ovunque; Piazza del Grano è «10 per ogni risposta corretta» (la mappa dice 0–40).
- Le posizioni x, y sono lette a occhio dalla slide della mappa: verificale sul posto. Le coordinate in basso a sinistra sono approssimative e solo decorative.
- Le foto sono quelle della presentazione: controlla che tu abbia i diritti per pubblicarle online.
- Non ho incluso la classifica in tempo reale.
