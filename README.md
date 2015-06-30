# babel-hubot [![npm version](https://badge.fury.io/js/babel-hubot.svg)](http://badge.fury.io/js/babel-hubot)

Minimalistic Hubot wrapper that allows to write scripts using power of ES2015.

## Installation

Install:

``` shell
npm install babel-hubot babel --save
```

Open local `bin/hubot` and replace regular `hubot` binary with `babel-hubot`
wrapper:

``` diff
--- a/bin/hubot
+++ b/bin/hubot
@@ -3,4 +3,4 @@
 npm install
 export PATH="node_modules/.bin:node_modules/hubot/node_modules/.bin:$PATH"

-exec node_modules/.bin/hubot "$@"
+exec node_modules/.bin/babel-hubot "$@"
```

## License

ngrok-daemon is released under the [MIT License](./LICENSE.md).

