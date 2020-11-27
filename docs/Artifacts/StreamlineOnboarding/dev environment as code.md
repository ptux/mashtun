# [WIP] dev environment as code

- Dockerfiles
- Automated IDE Setup

## What about our dev environments?

- A new developer gets pointed to the readme
- Reads lengthy, mostly outdated setup procedure
- Installs requirements on the developer machine, 
- updates/downgrades versions, etc.
- Tries to run the build … waits 20 minutes
- Build Fails. Try figure out what went wrong.
- Asks colleague. “Oh, yes. You also need to do X & Y”
- goto 3

## It works on my machine

If You Can't Reproduce a Bug, You Can't Fix It.

The situation when a bug only appears on one machine and is hard to reproduce on others.
That feeling when a bad thing happens in production, but you can’t reproduce it locally.
Not very surprising, though, as long you are running the code on a different platform based on a different setup.
