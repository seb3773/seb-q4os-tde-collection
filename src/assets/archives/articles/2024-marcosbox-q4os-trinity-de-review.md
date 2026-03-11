# Archived Article

**Original URL:** https://www.marcosbox.com/2024/01/16/q4os-trinity-de-review/  
**Source:** Marco's Box  
**Author:** Marco Giannini  
**Date:** January 16, 2024  
**Archived:** February 2025

---

# Q4OS – TRINITY DE REVIEW

**Author:** Marco Giannini  
**Date:** January 16, 2024  
**Tags:** BlackCodec, desktop environment, Informatica, Mondo Linux, q4os, Qt, Recensione, Trinity Desktop

---

Inizio subito con lo scusarmi per i modi in cui verrà affrontato l'argomento che probabilmente sembreranno non idonei ma capitemi, è la prima volta che faccio una review…

Oggi volevo riportarvi la mia esperienza con Q4OS e più in particolare con il desktop environment Trinity, non mi dilungo troppo sulle premesse e entriamo subito nel vivo.

## Q4OS

Q4OS è una distribuzione basata su Debian da cui eredita la stabilità (si appoggia infatti al ramo bookworm, attuale stable, con l'aggiunta dei repository proposed e backports) e il gran numero di pacchetti, aggiungedovi i propri attraverso alcuni repository custom.

Q4OS viene rilasciata sia col desktop environment KDE Plasma che con Trinity, su entrambe le release è presente un "Welcome Screen" e un "Software Centre", due tool che facilitano la vita dell'utente, soprattutto per i più novizi.

Il Software Centre consente all'utente di installare rapidamente le applicazioni più comuni quali browser, office ma anche vlc o i codec multimediali.

Sempre tramite il Software Centre è possibile installare anche Synaptic come interfaccia grafica per apt e scegliere quale profilo desktop utilizzare selezionando l'opzione Desktop Profiler.

Attenzione alla spunta **Remove superfluous packages** perché quando (e se) deciderete di cambiare profilo magari per passare da un full featured a un basic o minimal quel flag rimuoverà tutti i software non inclusi nel profilo selezionato. Questo significa che anche eventuali programmi aggiuntivi non inclusi nel profilo di destinazione che avete installato extra dal profilo "di provenienza" verranno rimossi.

Dalla stessa schermata, come si vede, è possibile cambiare e passare dal desktop environment Trinity a KDE Plasma e viceversa.

Selezionando il desktop profile che ci interessa e premendo sul pulsante Installazione (che diventerà cliccabile una volta selezionato un profilo desktop) si aprirà un'ulteriore schermata con l'avanzamento dell'installazione.

Se volessimo invece installare qualche programma direttamente dal Software Centre ci basterà fare doppio click sul programma scelto dalla lista e ci verrà mostrata una schermata simile a quella di un classico "setup alla Windows".

L'interfaccia è tradotta in italiano in quasi ogni sua parte anche nel wizard ma ogni tanto si nota una non corretta traduzione, passi per la descrizione in alto ma anche "Install" invece di "Installa", più che altro la non coerenza con gli altri pulsanti ("Indietro" e "Annulla") accentua maggiormente questo dettaglio.

Comunque anche l'installazione ricalca abbastanza fedelmente il classico wizard dei programmi installabili su windows.

Questo scimmiottamento del sistema di Redmond lo ritroviamo un po' ovunque anche nei temi (anche se magari potevano impegnarsi un pochino di più) e nel menu.

Per poi perdersi dove magari sarebbe stato più utile, ad esempio in LibreOffice è possibile impostare il tema simil Windows ma avrei gradito che fosse fatto out of the box.

E' possibile installare flatpak da riga di comando col solito `apt install flatpak` e aggiungere il repository di flathub per avere qualche applicazione in più aggiornata anche se il browser Firefox e Google Chrome (altra piacevole scoperta) sono già aggiornati all'ultima release, quindi non la LTS ma la release 121 al momento della scrittura.

## TRINITY DESKTOP ENVIRONMENT

E veniamo alla vera chicca della distribuzione, il desktop environment Trinity.

Guardate che bella che era l'interfaccia del vecchio Konqueror con il suo Control Centre.

Per tutti gli amanti del caro e buon vecchio KDE 3 sarà un bellissimo tuffo nel passato… un bellissimo amarcord… Per i più giovani sarà come vedere il genitore di quello che diverrà poi Plasma (si lo so che sotto al cofano è cambiato tutto ma non rovinatemi la vena di romanticismo).

### Perché cambiare? Perchééééé?!?!?!

Ok torniamo seri, Trinity è di fatto KDE 3 aggiornato alle Qt 4… in parte… e qui viene la nota dolente… Parliamo sempre di un desktop environment che poggia molte sue funzioni sulle Qt3 (il pacchetto tqt3 è indispensabile) e solamente nell'ultima release (attualmente la 14.1.1) ha effettivamente abbandonato Qt1 e Qt2.

Non che sia per forza un male ma onestamente siamo alle Qt6 e perfino LXQt sta lavorando al porting a questa versione… qui siamo ben 2 versioni indietro e ancora non è stato completato il porting?!

Tutto questo si traduce in un'esperienza utente veramente molto old old style, sembra quasi di utilizzare LXDE compilato in gtk2…

## COSA NON VA …

E ora veniamo alle note dolenti, i bug…

Il più spiacevole e veramente fastidioso è quello relativo al wizard, dopo aver infatti installato il software update manager e eseguito l'aggiornamento il wizard smette di visualizzare correttamente l'ultima schermata.

Ho provato anche ad eseguire una nuova installazione e il problema si ripresenta automaticamente dopo il primo apt upgrade… Non mi sono soffermato più di tanto sull'anomalia in quanto l'unica informazione che viene mostrata è la conferma di avvenuta installazione quindi quando si presenta la schermata possiamo tranquillamente chiuderla e confermare il kill al popup di avviso.

Per il resto è una Debian con qualche software leggermente più aggiornato (merito dei backports e dei proposed) e un tema che scimmiotta il vecchio Windows XP… Le icone non rispondono neanche lontanamente alle aspettative e (nonostante sia un'amante delle icone Crystal) risultano un po' datate, un po' come anche TDE in generale.

Il menu poi sinceramente non mi ha entusiasmato, anzi lo trovo veramente confusionario, nel tentativo di imitare il comportamento di Windows aggiunge layer che neanche in Win98 c'erano.

## CONCLUSIONI

La consiglierei? Onestamente sì il lavoro fatto dietro non è da poco e nonostante qualche bug o parte non tradotta non mi sento di dire che non sia valida, o almeno lo è quanto può essere una Debian.

Consiglierei Trinity come de? Sinceramente no, a parte i primi minuti con quell'effetto nostalgia tipica di chi ha amato KDE 3 poi onestamente ci si scontra con la sua arretratezza… Si bello ok ma nulla che faccia gridare al WOW, anzi sembra di vedere qualcosa di mooolto vecchio.

Certo se si cerca un DE completo che consumi poco allora forse effettivamente è qui che Trinity trova il suo parco utenza, alla fine il consumo a secco (senza applicazioni aperte o in esecuzione) è di poco meno di 500mb, certo non abbiamo effetti o animazioni ma normalmente chi opta per queste soluzioni se ne fa ben poco degli effetti speciali… tuttavia rimane la domanda ma se l'idea di un confronto vi stuzzica e avete apprezzato l'articolo fatecelo sapere nei commenti che potremmo provare a confrontarla con qualche altra distribuzione votata alla leggerezza, magari con LXQt o altre soluzioni che vi vengono in mente.

---

*This work is distributed under Creative Commons Attribution - Non Commercial - No Derivatives 4.0 International License.*
