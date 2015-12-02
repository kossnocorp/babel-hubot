# babel-hubot
[![npm version](https://badge.fury.io/js/babel-hubot.svg)](http://badge.fury.io/js/babel-hubot)

Minimalistic Hubot wrapper that allows to write scripts using power of ES 2015.

## Installation

Install (for Babel < 6, use `npm install babel-hubot#0.1 babel#5 --save`):

```shell
npm install babel-hubot babel-core coffee-script babel-preset-es2015 --save
```

Open local `bin/hubot` and replace regular `hubot` binary with `babel-hubot`
wrapper:

```diff
--- a/bin/hubot
+++ b/bin/hubot
@@ -3,4 +3,4 @@
 npm install
 export PATH="node_modules/.bin:node_modules/hubot/node_modules/.bin:$PATH"

-exec node_modules/.bin/hubot "$@"
+exec node_modules/.bin/babel-hubot "$@"
```

Then you might want to enable ES 2015, to do that, modify or create
`.babelrc` file:

```json
{
  "presets": ["es2015"]
}
```

## License

MIT
