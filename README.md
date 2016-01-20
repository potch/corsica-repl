# The Corsica REPL

Useful for sending content to screens and remotely managing their configuration.

At the bottom, an input for entering commands, at the top, command history.

## Commands

Commands start with either a URL, or a command type (e.g. `admin`), followed by space-separated `key=value` pairs.

Commands can be targeted to a screen with the screen dropdown. The dropdown can be overridden by specifying `screen=[screen]` in the command.

## Usage

Open it locally (or use the [hosted version](http://potch.github.io/corsica-repl/))

### Setup

Connect to a Corsica instance:

> repl server [server]

Be sure to use the fully qualified URL of the server, including protocol. Server information is stored in localStorage, so you should only have to do this when you change servers.

If you refresh the page, the dropdown should be populated with a list of screens connected to the server.

### Administration

To rename a screen:

> admin type=rename name=[name]

To subscribe a screen to a content tag:

> admin type=subscribe tag=[tag]

To un-subscribe a screen from a content tag:

> admin type=unsubscribe tag=[tag]

To reload a remote Corsica client:

> admin type=reload



