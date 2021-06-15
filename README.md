**Indice:** | [Chi Sono](#chi-sono) | [Progetti](#progetti)
> Attualmente sto lavorando ad una bot list italiana: https://primebots.it/

# Chi sono? <a name="chi-sono"></a>
Ciao, sono un giovane programmatore di 15 anni.<br>
Attualmente oserei dire che sono un Web Developer e un Discord Bot Developer.<br>
Mi sono focalizzato nella creazione di siti web dinamici con JavaScript sia dal lato server che client, con l'ausilio della libreria `express` e del runtime `Node.js`.<br>
Inoltre ho creato vari Chat Bot per Discord utilizzando sempre `Node.js` e la libreria `discord.js`. Ho provato anche a fare un libreria ([GoodBot](#GoodBot)) per velocizzare la creazione di bot per discord inserendola nel gestore di package [npm](https://www.npmjs.com/).<br>
Sicuramente il mio progetto che ha avuto più successo è [RockPaperScissors](#RockPaperScissors), un Bot per Discord che nel momento in qui lo scrivo è in 639 server


Ho scritto la mia prima riga di codice in pascal quando avevo 12 anni.<br>
Poi ho imparato le basi del Java con un corso su Udemy, passando per poco tempo su HTML e CSS.<br>
Per molto tempo poi mi sono focalizzato sul C# creando giochi su Unity e programmi desktop.<br>
Per un paio di mesi ho sperimentato il Python, ed infine mi sono focalizzato, prima, nella programmazione dei Bot per Discord, poi, anche nella creazione di siti web dinamici con `express`.


# Progetti <a name="progetti"></a>
Ecco i miei progetti degni di nota:
## <a name="RockPaperScissors">RockPaperScissors</a>
[![Discord Bots](https://top.gg/api/widget/servers/723877094920290305.svg)](https://top.gg/bot/723877094920290305)<br>
Un Bot per Discord che ho creato in JS (con `discord.js`) che attualmente è in 1300 server.<br>
Permette di far giocare a sasso carta forbici utente vs utente.<br>
Ecco vari link:<br>
* [Sito del bot](https://www.rps-bot.tk/) ([GitHub qui](https://github.com/AndreaGennaioli/rockpaperscissors-website))
* [Top.gg](https://top.gg/bot/723877094920290305)
* [dbots.co](https://dbots.co/bots/723877094920290305)
## <a name="GoodBot">GoodBot</a>
[![Discord Bots](https://nodei.co/npm/goodbot.png)](https://www.npmjs.com/package/goodbot)<br>
Un Framework per aiutare la creazione di Bot di Discord.<br>
Scritto in JavaScript e pubblicato come package su npm, vi lascio il [suo link di npmjs.com](https://www.npmjs.com/package/goodbot) per il download.<br>
Questo è il link per il suo [GitHub](https://github.com/AndreaGennaioli/GoodBot).<br>

Non è niente di serio (i download settimanali si aggirano sui 15, e totali sui 800) e l'ho fatto solo per vedere effettivamente come si creavano e pubblicavano package su npm.<br>

## <a name="captcha-api">Captcha Api (web api)</a>
E' una semplice web api che ho fatto per prova.<br>
Dopo aver fatto una richiesta a https://captchaapi.herokuapp.com/generator l'api rimandera indietro come risposta un'immagine (sfondo bianco con il codice scritto in nero) e il codice vero e proprio sotto forma di stringa.<br>
Ecco il link per il [GitHub](https://github.com/AndreaGennaioli/captcha-api) dove trovate anche la piccola documentazione.

Sempre scritto in JS, è un server fatto con `express` che, una volta aver fatto una richiesta GET a https://captchaapi.herokuapp.com/generator, con una semplice funzione random genera un codice. Poi viene creata anche un immagine usando la libraria `canvas` 200x100px con sfondo bianco e codice nero scritto sopra, salvandola in un file `.png` all'interno della cartella `captcha/` del server. In fine il server come risposta manda un oggetto JSON contenente il link all'immagine del captcha e il codice scritto in stringa.
