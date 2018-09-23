# ![RealWorld Example App](https://cloud.githubusercontent.com/assets/556934/25448178/3e7dc5c0-2a7d-11e7-8069-06da5169dae6.png)

👉 I gave [a talk](https://www.youtube.com/watch?v=x1FU3e0sT1I)
to explain the principles I used to build this. I highly recommend watching it!

> [Elm](http://elm-lang.org) codebase containing real world examples (CRUD, auth, advanced patterns, etc) that adheres to the [RealWorld](https://github.com/gothinkster/realworld-example-apps) spec and API.

### [Demo](https://elm-spa-example.netlify.com/)&nbsp;&nbsp;&nbsp;&nbsp;[RealWorld](https://github.com/gothinkster/realworld)

This codebase was created to demonstrate a fully fledged fullstack application built with [Elm](http://elm-lang.org) including CRUD operations, authentication, routing, pagination, and more.

For more information on how this works with other frontends/backends, head over to the [RealWorld](https://github.com/gothinkster/realworld) repo.

# How it works

Check out [the full writeup](https://dev.to/rtfeldman/tour-of-an-open-source-elm-spa)!

# Building

I decided not to include a build script, since all you need for a development build is the `elm` executable, and all you need on top of that for production is Uglify.

## Development Build

[Install Elm](https://guide.elm-lang.org/install.html) (e.g. with `npm install --global elm`), then from the root project directory, run this:

```
$ elm make src/Main.elm --output elm.js
```

If you want to include the time-traveling debugger, add `--debug` like so:

```
$ elm make src/Main.elm --output elm.js --debug
```

To view the site in a browser, bring up `index.html` from any local HTTP server, for example [`http-server`](https://www.npmjs.com/package/http-server).
