# sbundle-repo

Package repository for Sunbundler: a package manager for shortcuts. It can install packages with recursive dependencies. It lets you install and uninstall packages containing shortcuts, shell scripts, and javascript files.

## Installation

Read about how to install Sunbundler in `INSTALL.md`.

## Creating sbundles

To create sbundles, use the project editor included with ShortTerm. You can either run sbundlerX.X.X directly + enter the project's path, or run `$SB project editor ./project`. This will launch the editor. If the project doesn't exist yet, it will prompt you to create it. Then you can edit it with a UI menu.

If you prefer to edit from the command line, use 
- `$SB project create app ./project 1.0.0 project1.0.0 projectLatest`: to create an app (or replace app with library to create a library)
- `$SB project archive ./project` to create a sbundle archive of it
- `$SB project update ./project 1.0.1 project1.0.1` to update it to a new version.
- `$SB edit ./project/src/filename` to edit a file

## .sbundle format:
 sbundles are renamed .zip files with the contents:
 - apps.json: { "apps": [ { "title": "appname", "id": "appbundleidentifier", "store": "appstoreurl" } ... ] }
 - version.json: { "name": "packname", "num": "packver", "usid": "packshortcutname", "islib": true/false, "author": "your name", "created": "creation date", "updated": "update date", "get-latest": "https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/usid/latest.txt", "update": "https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/usid/usidLatest.sbundle", "datafold": "package's data folder location relative to shortcuts"}
 - README.md: package README file
 - lib/file/, lib/web/, bin/file/, bin/web/: required shortcuts either as `.shortcut` files (file) or iCloud links as `.txt` (web). The `file` folders can also contain shell scripts and javascript files.
 - deps/: group of required `.sbundle` files
 - data/: initial data folder contents

Note that the only required file is `version.json`. 
For a concrete example, see libHelloWorld or helloWorld.

## future plans

* A UI library using html and uuid tabs and shortcuts:// callbacks.

## bugs

Report all bugs in the issues tab.
