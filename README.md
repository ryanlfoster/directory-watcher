Directory Watcher
=================

Modified Java directory watcher example, made to be generic and useful.

## Changes

- Allow for a callback to be executed when a file/directory event is triggered
- Allow for path filtering from commandline
- Allow for notifications to be passed to executables (%file% and %event%)

## Example
```sh
java -jar DirectoryWatcher.jar -watch /Users/joshes/test -filter ".*?sub_dir\/?.*?" -callback "echo '%event% - %file%'"
```

[![Build Status](https://travis-ci.org/joshes/directory-watcher.svg?branch=master)](https://travis-ci.org/joshes/directory-watcher)