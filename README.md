# Welcome to typescript-agi-ng 👋

This piece of code is taken from https://github.com/fabiotheo/typescript-agi , which itself has been taken from https://github.com/brandonlehmann/typescript-agi

## Install

```sh
npm install typescript-agi-ng
```

## Run tests

```sh
npm run test
```

## Example Usage

```typescript
import {
    AGIServer, 
    Channel
} from 'typescript-agi-ng';

const agiServer = new AGIServer();

agiServer.on('channel', async(channel: Channel) => {
    await channel.answer();
    await channel.sayNumber(12345);
    await channel.hangup();
});

agiServer.start();
```
