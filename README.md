# stello

> Like map (and reduce) for [Trello](https://trello.com/) cards.


## Installation

Install from npm:

```
npm install -g stello
```


## Usage (cli)

Kick everything off:

`stello init`

You now have a stellorc config file in your working directory as well as some
source templates and template helpers.

`stello build`

Each card from your trello board gets mapped through the index template and
written to a `dist` directory.


## Usage (api)

Require `'stello'` and do your thing.

```javascript
var stello = require('stello');

stello.init({
  trelloApiKey: '36b098cd2f27e59119805f49468cbe60',
  trelloBoardUrl: 'https://trello.com/b/u4YdciVy/stello-boilerplate',
  trelloToken: '06e598e6521e837bb3c9b7db6a6519dc48348b9ef97f8b186929c239f2d531fe',
}, function(err){/* check for err */});

// `init` saves configs in `.stellorc` file

stello.build({
  // ... Optional, pass configs or use .stellorc file
}, function(err){/* check for err */});
```


## Release history

*(nothing yet)*


## Contributing

Please do! All I ask is that you create an issue before working on unsolicited
new features.


## License

[MIT](https://raw.github.com/jtrussell/stello/master/LICENSE-MIT)
