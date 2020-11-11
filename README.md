**Indice:** | [Chi Sono](#chi-sono) | [Progetti](#progetti)

# Chi sono? <a name="chi-sono"></a>
Ciao, sono un giovane programmatore di 15 anni.<br>
Attualmente oserei dire che sono un Web Developer e un Discord Bot Developer.<br>
Mi sono focalizzato nella creazione di siti web dinamici con JavaScript sia dal lato server che client, con l'ausilio della libreria `express` e del runtime `Node.js`.<br>
Inoltre creao Chat Bot per Discord utilizzando sempre `Node.js` e la libreria `discord.js`. Ho provato anche a fare un libreria ([GoodBot](#GoodBot)) per velocizzare la creazione di bot per discord inserendola nel gestore di package [npm](https://www.npmjs.com/).<br>
Sicuramente il mio progetto che ha avuto più successo è [RockPaperScissors](#RockPaperScissors), un Bot per Discord che nel momento in qui lo scrivo è in 639 server


Ho scritto la mia prima riga di codice in pascal quando avevo 12 anni.<br>
Poi ho imparato le basi del java con un corso su Udemy, passando per poco tempo su html e css.<br>
Per molto tempo poi mi sono focalizzato sul C# creando giochi su Unity e programmi desktop.<br>
Per un paio di mesi ho sperimentato il python, ed infine mi sono focalizzato, prima, nella programmazione dei Bot per Discord, poi, anche nella creazione di siti web dinamici con `express`.


# Progetti <a name="progetti"></a>
## <a name="RockPaperScissors">RockPaperScissors</a>
Un Bot per Discord che ho creato in JS che attualmente è in 639 server.<br>
Permette di far giocare a sasso carta forbici utente vs utente.<br>
[![Discord Bots](https://top.gg/api/widget/723877094920290305.svg)](https://top.gg/bot/723877094920290305)
## <a name="GoodBot">GoodBot</a>
GoodBot is a simple framework for building discord bots in JS.
<details>
  <summary style="display:flex"><strong>Installation</strong></summary>

Use the package manager [npm](https://www.npmjs.com/) to install goodbot.

```bash
npm install goodbot
```
</details>

<details>
  <summary><strong>Usage</strong></summary>




#### To initialize the bot:

```js
const { Client } = require("goodbot"); // importing goodbot
const path = require("path"); // importing path

const client = new Client({
  prefix: "!", // the bot's prefix
  ownerID: "465905397874688000", // your discord user id
  inviteLink: "https://discord.gg/botinvite", // the invite for your bot
  commandsFolder: path.join(__dirname, "commands"), // the commands folder, You need to make It
});

client.start("token"); // to start the bot with the token
```

#### To create Commands:

```js
// to create commands You first need to make Categories
client.addCommandsCategory("name", "description"); // to create 1 category

// to create more than 1 categories at once
client.addCommandsCategories([
  ["moderation", "moderation commands"],
  ["music", "music commands"],
]);

// You need to create a folder inside the commandsFolder for each category
```

After that you need to make a file for the command inside one of the categories folders.
Then to make the command write this in the command's file:

```js
module.exports = {
  name: "ping", // command name
  description: "ping command description", // command description
  argsType: 'multiple', // not required
  // argsType set the 'args' parameter options,
  // 'single' => all the args in a single string
  // 'multiple' => all the args in a string array

  run: (client, message, args) => {
    message.channel.send("Pong!");
    // ...
  },
};
```
</details>

<details>
  <summary><strong>More</strong></summary>


#### Default help command
To use the default help command:
```js
client.createDefaultHelp();
```

### Get a commandCategory
How to get a commandCategory:
```js
client.commandsCategories.get('moderation');
```

### Get a command
How to get a command:
```js
client.commandsCategories.get('moderation').get('ban');
```
</details>
