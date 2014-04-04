skeleton-project
================

A skeleton project for starting to build XMPP projects using XMPP-FTW


setup:
------
once checked out run:

```npm i```

...to install dependencies, then,

```npm start```

...which will start a server on port 3000

Then visit [http://localhost:3000](http://localhost:3000)

How it works

```
  +---------+  HTML/IMG/JS/CSS  +----------+
  | User /  | <---------------+ | xmpp-ftw |
  | Browser |      websocket    | server   |
  +---------+ <---------------> +----------+
                                    ^
                                    | socket
                                    |
                                    v
                                +--------+   component   +------------+
                                |  XMPP  |   connection  | buddycloud |
                                | server |<------------->| component  |
                                +--------+               +------------+
                                   + ^
                                   | |
                                   v +
                               +----------+
                               | External |
                               |   XMPP   |
                               |  server  |
                               +----------+
```
