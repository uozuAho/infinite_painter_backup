# Infinite Painter android backup

Syncs projects from infinite painter (android only) to your desktop.

Also creates links in the same structure as your folders on infinite painter,
making your projects easier to browse with a file explorer.

# quick start
Install python3 + rsync
run `./baktab <PROJECTS_DIR> <DEST_DIR>`

On my machine + tablet:
PROJECTS_DIR = "/run/user/1000/gvfs/mtp:host=MY_TABLET/Tablet/Android/data/com.brakefield.painter/files/Infinite Studio/Painter/Projects"
DEST_DIR = wherever I'm backing up to.

# dev
- test: original -> backup1. changed version -> backup2, then `diff -r backup1 backup2`
- lint:   `uvx ruff check baktab`
- format: `uvx ruff format --config indent-width=2 baktab`

# todo
- push
