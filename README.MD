# Canvamoji

node-canvas with support for discord and twitter based unicode emoji's.

## Installation
```shell
$ npm install canvamoji
```

## Quick Example
```javascript
const { createCanvas } = require('canvas');
const { fillTextWithTwemoji } = require('canvamoji');

async function main () {
    const canvas = createCanvas(200, 200);
    const context = canvas.getContext('2d');

    context.fillStyle = '#7289da';
    context.font = '30px Roboto';
    await fillTextWithTwemoji(context, 'emoji 😏 or discord emoji <:specssmart:797410575952379914>', 100, 100);
}

main();
```

## Dependencies

- node-canvas [GitHub](https://github.com/Automattic/node-canvas)
- twemoji-parser [GitHub](https://github.com/twitter/twemoji-parser)

## Licence

### node-canvas-with-twemoji

Copyright to people who own the dependencies.

Code licensed under the MIT License: http://opensource.org/licenses/MIT