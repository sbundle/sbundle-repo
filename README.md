# Sunbundler: Alpha 1.0.0

Sunbundler is an extractor for .sbundle (shortcut bundle) packages. It can install packages with recursive dependencies. It lets you install (uninstallation and creation are not implemented yet) executables and libraries.

## installation

Inside the shortcuts app, create two folders; one called bin and the other called lib. Then, download 
 these iCloud shortcuts:
 - https://www.icloud.com/shortcuts/9ccf949ef19b45dd89be2ef6ef5ba209
 - https://www.icloud.com/shortcuts/3103431ec7a14fecbf1111e6a4e4ec28
 - https://www.icloud.com/shortcuts/98f48c04ca4d4910acd4b4f9a8319f9d

To complete installation, run 'Sunbundler installer.' After that, you can install .sbundle files with the Sunbundler shortcut.

## how to install packages

Download the .sbundle file, such as lib/sbundles/helloWorld/helloWorldLatest.sbundle. Run 'Sunbundler,' and select the file you downloaded. After it completes, run 'Sunbundler install helper' over and over again until the installation is complete. Then you can use it (for example, run bin/helloWorldX.Y.Z).

## .sbundle format:
 sbundles are renamed .zip files with the contents:
 - apps.json: { "apps": [ { "title": "appname", "id": "appbundleidentifier", "store": "appstoreurl" } ... ] }
 - version.json: { "name": "packname", "num": "packver", "usid": "packshortcutname", "islib": true/false, "author": "your name", "created": "creation date", "updated": "update date", "get-latest": "https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/usid/latest.txt", "update": "https://github.com/sbundle/sbundle-repo/raw/refs/heads/main/lib/sbundles/usid/usidLatest.sbundle", "datafold": "package's data folder location relative to shortcuts"}
 - README.md: package README file
 - lib/file/, lib/web/, bin/file/, bin/web/: required shortcuts either as .shortcut files (file) or iCloud links as .txt (web)
 - deps/: group of required .sbundle files
 - data/: initial data folder contents

For a concrete example, see libHelloWorld or helloWorld.

## future features

The plan for the future is to support .js files as well as .shortcut files and include a linker for javascript "module" files. This will easily plug into shortcuts.

## bugs

Report all bugs in the issues tab.