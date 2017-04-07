# api documentation for  [node-twitterbot (v0.2.2)](http://www.projectspong.com/portfolio-type/nodebitlyapi/)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-twitterbot.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-twitterbot) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-twitterbot.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-twitterbot)
#### A NodeJS module for creating Twitter Bots

[![NPM](https://nodei.co/npm/node-twitterbot.png?downloads=true)](https://www.npmjs.com/package/node-twitterbot)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-twitterbot/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-twitterbot_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-twitterbot/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-twitterbot/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-twitterbot/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nathaniel Kirby",
        "email": "nate@projectspong.com",
        "url": "http://www.projectspong.com"
    },
    "bugs": {
        "url": "https://github.com/nkirby/node-twitterbot/issues",
        "email": "nate@projectspong.com"
    },
    "dependencies": {
        "twit": "~1.1.11"
    },
    "description": "A NodeJS module for creating Twitter Bots",
    "devDependencies": {
        "grunt": "~0.4.2",
        "grunt-banner": "~0.2.0",
        "grunt-contrib-coffee": "~0.8.2",
        "grunt-contrib-watch": "~0.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "145d5323757ef6a380443ceac11763b54a09d588",
        "tarball": "https://registry.npmjs.org/node-twitterbot/-/node-twitterbot-0.2.2.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "homepage": "http://www.projectspong.com/portfolio-type/nodebitlyapi/",
    "keywords": [
        "twitter",
        "bot"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/nkirby/node-twitterbot/blob/master/LICENSE"
        }
    ],
    "main": "lib/twitterbot.js",
    "maintainers": [
        {
            "name": "thenatekirby",
            "email": "nate@projectspong.com"
        }
    ],
    "name": "node-twitterbot",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nkirbygr/node-twitterbot.git"
    },
    "version": "0.2.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-twitterbot](#apidoc.module.node-twitterbot)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBot (configOrFile)](#apidoc.element.node-twitterbot.TwitterBot)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotAction (action, owner)](#apidoc.element.node-twitterbot.TwitterBotAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotStreamAction ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction)
1.  object <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBot.prototype
1.  object <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotAction.prototype
1.  object <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotStreamAction.prototype

#### [module node-twitterbot.TwitterBot](#apidoc.module.node-twitterbot.TwitterBot)
1.  boolean <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBot (configOrFile)](#apidoc.element.node-twitterbot.TwitterBot.TwitterBot)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>EventEmitter ()](#apidoc.element.node-twitterbot.TwitterBot.EventEmitter)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>init ()](#apidoc.element.node-twitterbot.TwitterBot.init)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>listenerCount (emitter, type)](#apidoc.element.node-twitterbot.TwitterBot.listenerCount)
1.  number <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>__super__

#### [module node-twitterbot.TwitterBot.prototype](#apidoc.module.node-twitterbot.TwitterBot.prototype)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>actionWithName (actionName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.actionWithName)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>addAction (actionName, callback)](#apidoc.element.node-twitterbot.TwitterBot.prototype.addAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>allActions (groupName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.allActions)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>constructor (configOrFile)](#apidoc.element.node-twitterbot.TwitterBot.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>listen (name, match, action)](#apidoc.element.node-twitterbot.TwitterBot.prototype.listen)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>now (action, tweet)](#apidoc.element.node-twitterbot.TwitterBot.prototype.now)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>randomAction (groupName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.randomAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>randomWeightedAction (groupName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.randomWeightedAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>removeAction (actionName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.removeAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>schedule (action, timeout, tweet)](#apidoc.element.node-twitterbot.TwitterBot.prototype.schedule)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>setupTwit ()](#apidoc.element.node-twitterbot.TwitterBot.prototype.setupTwit)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>startStreaming ()](#apidoc.element.node-twitterbot.TwitterBot.prototype.startStreaming)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>stopStreaming ()](#apidoc.element.node-twitterbot.TwitterBot.prototype.stopStreaming)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>tweet (text, callback)](#apidoc.element.node-twitterbot.TwitterBot.prototype.tweet)

#### [module node-twitterbot.TwitterBotAction](#apidoc.module.node-twitterbot.TwitterBotAction)
1.  boolean <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotAction (action, owner)](#apidoc.element.node-twitterbot.TwitterBotAction.TwitterBotAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>EventEmitter ()](#apidoc.element.node-twitterbot.TwitterBotAction.EventEmitter)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotAction.init)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>listenerCount (emitter, type)](#apidoc.element.node-twitterbot.TwitterBotAction.listenerCount)
1.  number <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>__super__

#### [module node-twitterbot.TwitterBotAction.prototype](#apidoc.module.node-twitterbot.TwitterBotAction.prototype)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>constructor (action, owner)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>getWeight ()](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>group (groupName)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.group)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.init)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>isPartOfGroup (groupName)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.isPartOfGroup)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>now (tweet)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.now)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>schedule (timeout, tweet)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.schedule)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>ungroup (groupName)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.ungroup)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>weight (_weight)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.weight)

#### [module node-twitterbot.TwitterBotStreamAction](#apidoc.module.node-twitterbot.TwitterBotStreamAction)
1.  boolean <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotStreamAction ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.TwitterBotStreamAction)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>EventEmitter ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.EventEmitter)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.init)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>listenerCount (emitter, type)](#apidoc.element.node-twitterbot.TwitterBotStreamAction.listenerCount)
1.  number <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>__super__

#### [module node-twitterbot.TwitterBotStreamAction.prototype](#apidoc.module.node-twitterbot.TwitterBotStreamAction.prototype)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>constructor ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>getStreamPath ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.getStreamPath)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.init)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>listen (name, match, callback)](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.listen)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>setStreamPath (stream_path)](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.setStreamPath)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>start ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.start)
1.  [function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>stop ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.stop)



# <a name="apidoc.module.node-twitterbot"></a>[module node-twitterbot](#apidoc.module.node-twitterbot)

#### <a name="apidoc.element.node-twitterbot.TwitterBot"></a>[function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBot (configOrFile)](#apidoc.element.node-twitterbot.TwitterBot)
- description and source-code
```javascript
function TwitterBot(configOrFile) {
  var e;
  if (typeof configOrFile === "string") {
    try {
      this.config = JSON.parse(fs.readFileSync(configOrFile));
    } catch (_error) {
      e = _error;
      throw e;
    }
  } else {
    this.config = configOrFile;
  }
  this.actions = [];
  this.streamAction = new TwitterBotStreamAction(function() {
    return this.start();
  }, this);
  this.setupTwit();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotAction (action, owner)](#apidoc.element.node-twitterbot.TwitterBotAction)
- description and source-code
```javascript
function TwitterBotAction(action, owner) {
  var _this = this;
  this.owner = owner;
  this.on("action", function(twitter, tweet) {
    return action(twitter, _this, tweet);
  });
  this.init();
  this.groups = [];
  this._weight = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotStreamAction ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction)
- description and source-code
```javascript
function TwitterBotStreamAction() {
  _ref = TwitterBotStreamAction.__super__.constructor.apply(this, arguments);
  return _ref;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-twitterbot.TwitterBot"></a>[module node-twitterbot.TwitterBot](#apidoc.module.node-twitterbot.TwitterBot)

#### <a name="apidoc.element.node-twitterbot.TwitterBot.TwitterBot"></a>[function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBot (configOrFile)](#apidoc.element.node-twitterbot.TwitterBot.TwitterBot)
- description and source-code
```javascript
function TwitterBot(configOrFile) {
  var e;
  if (typeof configOrFile === "string") {
    try {
      this.config = JSON.parse(fs.readFileSync(configOrFile));
    } catch (_error) {
      e = _error;
      throw e;
    }
  } else {
    this.config = configOrFile;
  }
  this.actions = [];
  this.streamAction = new TwitterBotStreamAction(function() {
    return this.start();
  }, this);
  this.setupTwit();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.EventEmitter"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>EventEmitter ()](#apidoc.element.node-twitterbot.TwitterBot.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.init"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>init ()](#apidoc.element.node-twitterbot.TwitterBot.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.listenerCount"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.</span>listenerCount (emitter, type)](#apidoc.element.node-twitterbot.TwitterBot.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-twitterbot.TwitterBot.prototype"></a>[module node-twitterbot.TwitterBot.prototype](#apidoc.module.node-twitterbot.TwitterBot.prototype)

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.actionWithName"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>actionWithName (actionName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.actionWithName)
- description and source-code
```javascript
actionWithName = function (actionName) {
  var action, _i, _len, _ref;
  _ref = this.actions;
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    action = _ref[_i];
    if (action.name === actionName) {
      return action;
    }
  }
  return null;
}
```
- example usage
```shell
...

    var tweetAction = Bot.addAction("tweet", function(twitter, action, tweet) {
      Bot.tweet("I'm posting a tweet!");
    });

But you will rarely need to directly hold onto the tweetAction directly. You can always get a reference to the action by calling

    Bot.actionWithName("tweet");

Which will return the TwitterBotAction object, or null if the name is invalid (or the action already removed)

See more about the [TwitterBotAction class here](https://github.com/nkirby/node-twitterbot/wiki/TwitterBotAction "TwitterBotAction
 Wiki")

### Grouping Actions
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.addAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>addAction (actionName, callback)](#apidoc.element.node-twitterbot.TwitterBot.prototype.addAction)
- description and source-code
```javascript
addAction = function (actionName, callback) {
  var action,
    _this = this;
  if (typeof callback === "function") {
    action = new TwitterBotAction(callback, this);
  } else {
    action = callback;
  }
  action.name = actionName;
  this.actions.push(action);
  this.on(actionName, function(params) {
    return action.emit("action", params);
  });
  return action;
}
```
- example usage
```shell
...
In order to get your node-twitterbot to actually do something, you need to define actions. It is done through the addAction() method
. It takes 2 parameters:

    actionName: a string value for the name of an action
  	actionFunction: a function to be called when a given action is scheduled. (See below for method signature)

So our addAction method might look like this:

    Bot.addAction("tweet", function(twitter, action, tweet) {
      Bot.tweet("I'm posting a tweet!");
    });

The twitter variable passed into the function is the [Twit](https://github.com/ttezel/twit/ "Twit on Github") object associated
with a given node-twitterbot, and can be managed directly. The same Twit object is available as [TwitterBot].twitter as well.

The action variable passed into the function is the TwitterBotAction created by addAction.
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.allActions"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>allActions (groupName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.allActions)
- description and source-code
```javascript
allActions = function (groupName) {
  var action, actions, _i, _len, _ref;
  actions = [];
  _ref = this.actions;
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    action = _ref[_i];
    if (groupName) {
      if (action.isPartOfGroup(groupName)) {
        actions.push(action.name);
      }
    } else {
      actions.push(action);
    }
  }
  return actions;
}
```
- example usage
```shell
...

    Bot.addAction("tweet", function(twitter, action, tweet) {
      Bot.tweet("I'm posting a tweet!");
    }).group("tweet posting");

Retrieving all actions in a group is possible via:

    Bot.allActions("tweet posting");

A TwitterBotAction can be part of multiple groups.

### Randomizing Actions

If you create multiple actions for a given TwitterBot, you can get a random one back by calling
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.constructor"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>constructor (configOrFile)](#apidoc.element.node-twitterbot.TwitterBot.prototype.constructor)
- description and source-code
```javascript
function TwitterBot(configOrFile) {
  var e;
  if (typeof configOrFile === "string") {
    try {
      this.config = JSON.parse(fs.readFileSync(configOrFile));
    } catch (_error) {
      e = _error;
      throw e;
    }
  } else {
    this.config = configOrFile;
  }
  this.actions = [];
  this.streamAction = new TwitterBotStreamAction(function() {
    return this.start();
  }, this);
  this.setupTwit();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.listen"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>listen (name, match, action)](#apidoc.element.node-twitterbot.TwitterBot.prototype.listen)
- description and source-code
```javascript
listen = function (name, match, action) {
  return this.streamAction.listen(name, match, action);
}
```
- example usage
```shell
...
Bot.randomWeightedAction("tweet posting");


## Streaming

If you want to watch the Twitter timeline, you can use the built in TwitterBotStreamAction object. One is automatically provided
 for you as part of the TwitterBot.

Bot.listen(listenerName, listenerFunction, function(twitter, action, tweet) {
  // Do something with the tweet
});

The listenerName is a string that identifies the listener. The listenerFunction follows the following format:

listenerFunction = function(tweet) {
  if (something)
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.now"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>now (action, tweet)](#apidoc.element.node-twitterbot.TwitterBot.prototype.now)
- description and source-code
```javascript
now = function (action, tweet) {
  if (typeof action === "string") {
    action = this.actionWithName(action);
  } else if (typeof action === "function") {
    action = new TwitterBotAction(callback, this);
  }
  return action.emit("action", this.twitter, tweet);
}
```
- example usage
```shell
...
}

By returning true, you'll tell the listen() function to execute the passed callback method.

For example:

Bot.listen("listening", tweetThatContainsName, function(twitter, action, tweet) {
  Bot.now(Bot.randomWeightedAction("reply actions"), tweet);
});

Would cause our TwitterBot to perform some random action in the "reply actions" group, whenever the tweetThatContainsName() function
 returns true.

You can create a TwitterBotStreamAction via:

var streamAction = new TwitterBotStreamAction(null, Bot)
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.randomAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>randomAction (groupName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.randomAction)
- description and source-code
```javascript
randomAction = function (groupName) {
  var actionItem, actions;
  actions = this.allActions(groupName);
  actionItem = actions[Math.floor(Math.random() * actions.length)];
  return actionItem;
}
```
- example usage
```shell
...

A TwitterBotAction can be part of multiple groups.

### Randomizing Actions

If you create multiple actions for a given TwitterBot, you can get a random one back by calling

    Bot.randomAction();

If you want a random action in a group, you can pass in the group name

    Bot.randomAction("group name");

### Weighting Actions
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.randomWeightedAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>randomWeightedAction (groupName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.randomWeightedAction)
- description and source-code
```javascript
randomWeightedAction = function (groupName) {
  var action, i, weight, weightedActions, _i, _j, _len, _ref;
  weightedActions = [];
  _ref = this.actions;
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    action = _ref[_i];
    weight = action.getWeight();
    for (i = _j = 0; 0 <= weight ? _j <= weight : _j >= weight; i = 0 <= weight ? ++_j : --_j) {
      weightedActions.push(action.name);
    }
  }
  return weightedActions[Math.floor(Math.random() * weightedActions.length)];
}
```
- example usage
```shell
...

Bot.addAction("tweet", function(twitter, action, tweet) {
  Bot.tweet("I'm posting a tweet!");
}).group("tweet posting").weight(10);

You can then get a random action, taking the action weights into account, by calling:

Bot.randomWeightedAction("tweet posting");


## Streaming

If you want to watch the Twitter timeline, you can use the built in TwitterBotStreamAction object. One is automatically provided
 for you as part of the TwitterBot.

Bot.listen(listenerName, listenerFunction, function(twitter, action, tweet) {
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.removeAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>removeAction (actionName)](#apidoc.element.node-twitterbot.TwitterBot.prototype.removeAction)
- description and source-code
```javascript
removeAction = function (actionName) {
  var index;
  this.removeAllListeners(actionName);
  index = this.actions.indexOf(actionName);
  if (index > -1) {
    return this.actions.splice(index, 1);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.schedule"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>schedule (action, timeout, tweet)](#apidoc.element.node-twitterbot.TwitterBot.prototype.schedule)
- description and source-code
```javascript
schedule = function (action, timeout, tweet) {
  if (!timeout) {
    return this.now(action);
  }
}
```
- example usage
```shell
...
    });
    Bot.now(twitterBotAction);

The now() function takes either an actionName identifier, a function with the same signaure as a TwitterBotAction, or an actual
TwitterBotAction object

You can schedule actions into the future by calling

    Bot.schedule("action name", 1000);

Would cause the Bot's "action name" action to be called after 1000 ms (same as setTimeout)

### Rescheduling

Since the second parameter passed into the TwitterBotAction's method is the TwitterBotAction itself, you can call this:
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.setupTwit"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>setupTwit ()](#apidoc.element.node-twitterbot.TwitterBot.prototype.setupTwit)
- description and source-code
```javascript
setupTwit = function () {
  this.twitter = new Twit({
    consumer_secret: this.config.consumer_secret,
    consumer_key: this.config.consumer_key,
    access_token: this.config.access_token,
    access_token_secret: this.config.access_token_secret
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.startStreaming"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>startStreaming ()](#apidoc.element.node-twitterbot.TwitterBot.prototype.startStreaming)
- description and source-code
```javascript
startStreaming = function () {
  return this.streamAction.start();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.stopStreaming"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>stopStreaming ()](#apidoc.element.node-twitterbot.TwitterBot.prototype.stopStreaming)
- description and source-code
```javascript
stopStreaming = function () {
  return this.streamAction.stop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBot.prototype.tweet"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBot.prototype.</span>tweet (text, callback)](#apidoc.element.node-twitterbot.TwitterBot.prototype.tweet)
- description and source-code
```javascript
tweet = function (text, callback) {
  if (typeof text !== "string") {
    return callback({
      message: "Cannot post a non-string"
    }, null);
  }
  return this.twitter.post("statuses/update", {
    status: text
  }, function(err, response) {
    if (callback && typeof callback === "function") {
      return callback(err, response);
    }
  });
}
```
- example usage
```shell
...

    actionName: a string value for the name of an action
  	actionFunction: a function to be called when a given action is scheduled. (See below for method signature)

So our addAction method might look like this:

    Bot.addAction("tweet", function(twitter, action, tweet) {
      Bot.tweet("I'm posting a tweet!");
    });

The twitter variable passed into the function is the [Twit](https://github.com/ttezel/twit/ "Twit on Github") object associated
with a given node-twitterbot, and can be managed directly. The same Twit object is available as [TwitterBot].twitter as well.

The action variable passed into the function is the TwitterBotAction created by addAction.

And the tweet object is the tweet passed into the action (if there was one)
...
```



# <a name="apidoc.module.node-twitterbot.TwitterBotAction"></a>[module node-twitterbot.TwitterBotAction](#apidoc.module.node-twitterbot.TwitterBotAction)

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.TwitterBotAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotAction (action, owner)](#apidoc.element.node-twitterbot.TwitterBotAction.TwitterBotAction)
- description and source-code
```javascript
function TwitterBotAction(action, owner) {
  var _this = this;
  this.owner = owner;
  this.on("action", function(twitter, tweet) {
    return action(twitter, _this, tweet);
  });
  this.init();
  this.groups = [];
  this._weight = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.EventEmitter"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>EventEmitter ()](#apidoc.element.node-twitterbot.TwitterBotAction.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.init"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotAction.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.listenerCount"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.</span>listenerCount (emitter, type)](#apidoc.element.node-twitterbot.TwitterBotAction.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-twitterbot.TwitterBotAction.prototype"></a>[module node-twitterbot.TwitterBotAction.prototype](#apidoc.module.node-twitterbot.TwitterBotAction.prototype)

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.constructor"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>constructor (action, owner)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.constructor)
- description and source-code
```javascript
function TwitterBotAction(action, owner) {
  var _this = this;
  this.owner = owner;
  this.on("action", function(twitter, tweet) {
    return action(twitter, _this, tweet);
  });
  this.init();
  this.groups = [];
  this._weight = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>getWeight ()](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.getWeight)
- description and source-code
```javascript
getWeight = function () {
  return this._weight;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.group"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>group (groupName)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.group)
- description and source-code
```javascript
group = function (groupName) {
  this.groups.push(groupName);
  return this;
}
```
- example usage
```shell
...

### Grouping Actions

Actions are groupable by calling the TwitterBotAction objects group() method

    Bot.addAction("tweet", function(twitter, action, tweet) {
      Bot.tweet("I'm posting a tweet!");
    }).group("tweet posting");

Retrieving all actions in a group is possible via:

    Bot.allActions("tweet posting");

A TwitterBotAction can be part of multiple groups.
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.init"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.init)
- description and source-code
```javascript
init = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.isPartOfGroup"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>isPartOfGroup (groupName)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.isPartOfGroup)
- description and source-code
```javascript
isPartOfGroup = function (groupName) {
  return this.groups.indexOf(groupName) > -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.now"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>now (tweet)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.now)
- description and source-code
```javascript
now = function (tweet) {
  return this.owner.now(this, tweet);
}
```
- example usage
```shell
...
}

By returning true, you'll tell the listen() function to execute the passed callback method.

For example:

Bot.listen("listening", tweetThatContainsName, function(twitter, action, tweet) {
  Bot.now(Bot.randomWeightedAction("reply actions"), tweet);
});

Would cause our TwitterBot to perform some random action in the "reply actions" group, whenever the tweetThatContainsName() function
 returns true.

You can create a TwitterBotStreamAction via:

var streamAction = new TwitterBotStreamAction(null, Bot)
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.schedule"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>schedule (timeout, tweet)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.schedule)
- description and source-code
```javascript
schedule = function (timeout, tweet) {
  return this.owner.schedule(this, timeout);
}
```
- example usage
```shell
...
    });
    Bot.now(twitterBotAction);

The now() function takes either an actionName identifier, a function with the same signaure as a TwitterBotAction, or an actual
TwitterBotAction object

You can schedule actions into the future by calling

    Bot.schedule("action name", 1000);

Would cause the Bot's "action name" action to be called after 1000 ms (same as setTimeout)

### Rescheduling

Since the second parameter passed into the TwitterBotAction's method is the TwitterBotAction itself, you can call this:
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.ungroup"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>ungroup (groupName)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.ungroup)
- description and source-code
```javascript
ungroup = function (groupName) {
  var index;
  index = this.groups.indexOf(groupName);
  if (index > -1) {
    this.groups.splice(index, 1);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotAction.prototype.weight"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotAction.prototype.</span>weight (_weight)](#apidoc.element.node-twitterbot.TwitterBotAction.prototype.weight)
- description and source-code
```javascript
weight = function (_weight) {
  this._weight = _weight;
  return this;
}
```
- example usage
```shell
...

### Weighting Actions

If you want to make the randomAction function a little less random, you can give weights to all TwitterBotActions

    Bot.addAction("tweet", function(twitter, action, tweet) {
      Bot.tweet("I'm posting a tweet!");
    }).group("tweet posting").weight(10);

You can then get a random action, taking the action weights into account, by calling:

    Bot.randomWeightedAction("tweet posting");


## Streaming
...
```



# <a name="apidoc.module.node-twitterbot.TwitterBotStreamAction"></a>[module node-twitterbot.TwitterBotStreamAction](#apidoc.module.node-twitterbot.TwitterBotStreamAction)

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.TwitterBotStreamAction"></a>[function <span class="apidocSignatureSpan">node-twitterbot.</span>TwitterBotStreamAction ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.TwitterBotStreamAction)
- description and source-code
```javascript
function TwitterBotStreamAction() {
  _ref = TwitterBotStreamAction.__super__.constructor.apply(this, arguments);
  return _ref;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.EventEmitter"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>EventEmitter ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.init"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.listenerCount"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.</span>listenerCount (emitter, type)](#apidoc.element.node-twitterbot.TwitterBotStreamAction.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-twitterbot.TwitterBotStreamAction.prototype"></a>[module node-twitterbot.TwitterBotStreamAction.prototype](#apidoc.module.node-twitterbot.TwitterBotStreamAction.prototype)

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.constructor"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>constructor ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.constructor)
- description and source-code
```javascript
function TwitterBotStreamAction() {
  _ref = TwitterBotStreamAction.__super__.constructor.apply(this, arguments);
  return _ref;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.getStreamPath"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>getStreamPath ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.getStreamPath)
- description and source-code
```javascript
getStreamPath = function () {
  return this.stream_path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.init"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>init ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.init)
- description and source-code
```javascript
init = function () {
  var _this = this;
  this.streams = {};
  this.on("start", function() {
    return _this.start();
  });
  this.on("stop", function() {
    return _this.stream.stop();
  });
  return this.stream_path = "statuses/sample";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.listen"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>listen (name, match, callback)](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.listen)
- description and source-code
```javascript
listen = function (name, match, callback) {
  var action,
    _this = this;
  action = new TwitterBotAction(callback, this.owner);
  this.streams[name] = match;
  return this.on("stream-" + name, function(twitter, tweet) {
    return action.emit("action", twitter, tweet);
  });
}
```
- example usage
```shell
...
Bot.randomWeightedAction("tweet posting");


## Streaming

If you want to watch the Twitter timeline, you can use the built in TwitterBotStreamAction object. One is automatically provided
 for you as part of the TwitterBot.

Bot.listen(listenerName, listenerFunction, function(twitter, action, tweet) {
  // Do something with the tweet
});

The listenerName is a string that identifies the listener. The listenerFunction follows the following format:

listenerFunction = function(tweet) {
  if (something)
...
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.setStreamPath"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>setStreamPath (stream_path)](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.setStreamPath)
- description and source-code
```javascript
setStreamPath = function (stream_path) {
  this.stream_path = stream_path;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.start"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>start ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.start)
- description and source-code
```javascript
start = function () {
  var _this = this;
  this.stream = this.owner.twitter.stream(this.stream_path);
  this.stream.on("tweet", function(tweet) {
    var key, value, _ref1;
    _ref1 = _this.streams;
    for (key in _ref1) {
      value = _ref1[key];
      if (value(tweet)) {
        _this.emit("stream-" + key, _this.owner.twitter, tweet);
      }
    }
    return tweet;
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.stop"></a>[function <span class="apidocSignatureSpan">node-twitterbot.TwitterBotStreamAction.prototype.</span>stop ()](#apidoc.element.node-twitterbot.TwitterBotStreamAction.prototype.stop)
- description and source-code
```javascript
stop = function () {
  return this.emit("stop");
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
