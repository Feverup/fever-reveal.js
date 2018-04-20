# READMEFEVER.md

## Run the server in a Docker container

- Go to the repository root.
- Run:

```bash
$ docker run --rm -ti -v `pwd`:/app -u $UID:$GROUPS -p 8000:8000 node /bin/bash
$ cd app
$ npm install
$ npm start
```

Browse to http://localhost:8000/slides/_your-talk-name_ to see your slides.

## Editing the repository

Please, to ease the tracking of the original repository, limits you edits to
the next files and folders:

- slides/_your-talk-name_ (each talk has its own folder under slides/).
- css/theme/fever.css (the theme for our slides).

The Docker image mounts the repository in the container. You can make changes
directly to the files and update the browser.

## Images and other binary resources

Create a `bin/` folder under you talk folder and use Google Drive to manage
this files. Don't upload binary files to this repository.

