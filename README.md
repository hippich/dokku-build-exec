dokku-build-exec
================

Inject build commands to be run in pre-build stage.

dokku-build-exec is a plugin for [dokku][dokku] that runs custom script your dokku environment.
This is mostly useful for instances where you have an app that depends on custom environment.

## Installation

On your dokku server:

### dokku >= 0.4.0
```sh
sudo dokku plugin:install https://github.com/hippich/dokku-build-exec
```

## Usage

When you deploy your project, the dokku-build-exec plugin will run `.build-exec` shell script.
Make sure to make that script executabe and use correct shebang.

[dokku]: https://github.com/progrium/dokku
