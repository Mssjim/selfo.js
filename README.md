<div align="center">
  <br />
  <p>
    <img src="./logo.png" width="800" alt="selfo.js" />
  </p>
  <br />
  <p>
    <a href="https://www.npmjs.com/package/selfo.js"><img src="https://img.shields.io/npm/v/selfo.js.svg?maxAge=3600" alt="NPM version" /></a>
    <a href="https://www.npmjs.com/package/selfo.js"><img src="https://img.shields.io/npm/dt/selfo.js.svg?maxAge=3600" alt="NPM downloads" /></a>
    <a href="https://github.com/Mssjim/selfo.js"><img src="https://badge.fury.io/gh/Mssjim%2FDragon-Animes.svg" alt="GitHub Version" /></a>
    <a href="https://github.com/Mssjim/selfo.js/blob/master/LICENSE"><img src="https://img.shields.io/github/license/Mssjim/Dragon-Animes.svg" alt="GitHub Version" /></a>
  </p>
  <p>
    <a href="https://nodei.co/npm/selfo.js/"><img src="https://nodei.co/npm/selfo.js.png?downloads=true&stars=true" alt="NPM info" /></a>
  </p>
</div>

## About
selfo.js is an personal [node.js](https://nodejs.org) module that allows you to interact with the
[Discord API] (https://discordapp.com/developers/docs/intro) focusing on self-bot accounts.

- Object-oriented
- Predictable abstractions
- Performant
- 100% coverage of the Discord API

## Warning
Selfbots **violate Discord TOS and Discord-Bots TOS**. Be careful about how you use this module and use at your risk.

## Installation
Ignore any warnings about unmet peer dependencies, as they're all optional.

- Without voice support: `npm install selfo.js`  
- With voice support ([node-opus](https://www.npmjs.com/package/node-opus)): `npm install selfo.js node-opus`

## Example usage
```js
const { Client } = require('selfo.js');
const selfo = new Client();

selfo.on('ready', () => {
  console.log(`Logged in as ${selfo.user.tag}!`);
});

selfo.on('message', msg => {
  if (msg.content == 'ping')
    msg.reply('pong');
});

selfo.login('ACCOUNT TOKEN');
```

### Links
* [Source](https://github.com/Mssjim/selfo.js)
* [NPM](https://www.npmjs.com/package/selfo.js)

### Discord.js Links
* [Website](https://discord.js.org/)
* [Documentation](https://discord.js.org/#/docs)
* [GitHub](https://github.com/discordjs/discord.js)
* [NPM](https://www.npmjs.com/package/discord.js)

### Extensions
* [RPC](https://www.npmjs.com/package/discord-rpc) ([source](https://github.com/discordjs/RPC))

## Contributing
Before creating an issue, please ensure that it hasn't already been reported or suggested.