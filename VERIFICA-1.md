# VERIFICA TPSI: AWS, HTML5, deploy

Benvenuti alla verifica scritta di TPSI. Buon lavoro!

## Panoramica del compito
Il compito è diviso in tre fasi:
1. avvio di una macchina EC2 su AWS
1. modifica di una pagina web in locale
1. deploy della pagina web sull'istanza EC2

Wireframe: [https://wireframe.cc/pro/pp/a3fa2da93288625](https://wireframe.cc/pro/pp/a3fa2da93288625)
## Operazioni preliminari
Accesso ad AWS:
- accedete alla [pagina di login](https://www.awseducate.com/signin/SiteLogin) di AWS Educate
- quando create una nuova istanza, **create una nuova chiave** con il nome **cognome-verifica**; questa chiave dovete metterla sotto revisione su github in modo che io possa accedere alla vostra istanza!
- per le operazioni di configurazione potete usare gli appunti a [questo](https://github.com/wbigger/tpsi-5y/) indirizzo

Sviluppo web locale:
- accedete con il vostro account personale a GitHub (**non sbagliate password!**)
- fate il fork di questo progetto, ma **attenzione**: se vi viene chiesto, fate il fork sul vostro account personale e non sull'organizzazione del progetto di classe
- copiate l'URL del **vostro** progetto
- aprite Visual Studio Code
- fate il clone del progetto
- premete sul pulsante "Go Live" nella barra blu in basso
- a questo punto avete la pagina di riferimento aperta sul vostro browser e potete cominciare lo sviluppo

## Note
Attenzione: alla fine della verifica, **non** fermate o terminate l'istanza da voi generata perché mi servirà per la correzione!

Testate il vostro progetto il più spesso possibile per controllare che non sia corretto.

**È possibile** consultare w3school o altri siti di esempio.

Al contrario, **non è possibile** comunicare o copiare dai compagni di classe.

Almeno 5 minuti prima della fine verifica, fate il commit e push di tutte le modifiche in locale. Consigliamo comunque di fare commit e push molto spesso durante la verifica (anche ogni 10 minuti), per evitare di perdere punti.

## Calcolo del punteggio
Tutte le seguenti voci valgono **1 punto**.
Voto massimo: 10.
Per avere il massimo del voto bisogna avere il massimo del punteggio.


### Punti generali
- [X] corretta indentazione di tutti i file
- [X] codice che compila senza errori nella console del browser

### Parte prima: AWS
- [X] creare una istanza Amazon Linux 2 con architettura x86 a 64 bit
- [X] creare una istanza per uso generale, che abbia almeno 2GB di RAM e senza particolari requisiti per la CPU, lo storage e le prestazioni di rete
- [X] configurare l'istanza in modo da accettare chiamate HTTP, HTTPS e MYSQL (quest'ultima accessibile solo dal mio IP)
- [X] connettersi all'istanza e configurare il web server nginx
- [X] la pagina di default del web server è correttamente visulizzata nel browser del proprio computer di sviluppo

### Parte seconda: sviluppo web in locale
- [X] modifica del titolo della pagina in "Visita Civitavecchia"
- [X] heading principale e relativo sottotitolo corretto
- [X] una immagine del forte con descrizione corretta
- [/] tutte e tre le immagini del forte e descrizioni corrette
- [X] crezione di due screenshots, uno per desktop e uno per smartphone, da caricare su github
- [X] corretta capitalizzazione di tutti i testi
- [ ] sostituire l'immagine di background con il video a [questo link](https://visit-civitavecchia.s3-eu-west-1.amazonaws.com/Stone-Falls.mp4), che si riproduca inline, abbia l'autoplay, sia muto (muted) e a loop (vedi la [documentazione ufficiale](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video) di MDN)
- [ ] quando viene premuto il tasto "Scopri di più", va alla sezione about
- [ ] quando viene premuto il tasto "Guarda il video", viene chiamata la funzione "lightbox_open();"
- [ ] seguendo [questo](https://developer.mozilla.org/en-US/docs/Web/Guide/Audio_and_video_delivery/Adding_captions_and_subtitles_to_HTML5_video) tutorial, aggiungere i sottotitoli in inglese al video.

### Parte terza: deploy
- [X] download del progetto web sull'istanza
- [X] corretto deploy del sito nell'istanza
- [X] pagina visualizzabile da browser con dns pubblico


