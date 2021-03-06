Riot ConnectN
===============

A simple and flexible implementation on the connect4 game http://en.wikipedia.org/wiki/Connect_Four.

This APP uses riotjs (https://muut.com/riotjs/) framework but the main logic is compleatly decoupled from any framework, so it can be used with any framework on nodejs or the browser. Riotjs is a very minimal (1k) framework that give us just the `observeble`, `render` and `bdd`.

## Try the APP

Just visit http://www.3den.org/riotjs-connect4/ or clone the app and open `index.html` in you favorite browser.

## Tests

I am using Riot's BDD framework, which I built myself, it is very minimal, promotes custom assertions and can run on nodejs or the browser.

To run the tests on the command line you can use make:

```
$ make
```

or run the node test manually:

```
$ node test/node.js
```

I you prefer, you can also run the tests on the browser, just open `test/index.html` and check the browser console.

## About the Code

The business logic of ConnectN is in `lib/connect_n.js` and it is fully tested in `test/connect_n_test.js`. The code should be simple to understand, it uses
prototypal inheritance instead of pseudo-classical.

In the `app` directory you will see that the logic that depends on riotjs and the DOM, even tho I love jQuery there was no need for it, yay!
