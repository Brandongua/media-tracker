# Media Library Management System

A tracker for all of your media. Books, games, movies, and more.
This is just the api, it is likely you would want a client, such as the
[web client](https://github.com/brandongua/media-tracker-web)


## Purpose

There are many trackers online, but they only track just shows, or just books
etc... In addition you can't add custom items to them. With this program
you can add anything you want, such as:
* games
* movies
* tv shows
* books
* albums
* individual songs
* specific game endings
* specific chapters in a book

### Running

> [!NOTE]
Only tested on linux

> [!TIP]
To use the omdb provider, get an omdb key and export the OMDB_KEY variable

> [!TIP]
To use the wikipedia provider, export the WIKI_EMAIL variable to your email

```bash
git clone https://github.com/brandongua/media-tracker-api

cd media-tracker-api

./build

./mediatracker
```

A server will then be running on `localhost:8080`

### Configuration

By default things are stored in `$AIO_DIR` which by default is `$XDG_DATA_HOME/media-tracker`

Each user has their own directory in the `/users` folder in `$AIO_DIR`. Their folder will be their user id.

Each user gets their own `settings.json` file.

### Docs
Basic api documentation can be found at `/docs`

Basic user facing docs can be found at `/usage`


### Clients

[implementing a client](./CLIENTS.md)
