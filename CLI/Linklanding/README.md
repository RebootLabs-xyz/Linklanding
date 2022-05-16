oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g Linklanding
$ Linklanding COMMAND
running command...
$ Linklanding (--version)
Linklanding/0.0.0 linux-x64 node-v16.14.2
$ Linklanding --help [COMMAND]
USAGE
  $ Linklanding COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`Linklanding hello PERSON`](#linklanding-hello-person)
* [`Linklanding hello world`](#linklanding-hello-world)
* [`Linklanding help [COMMAND]`](#linklanding-help-command)
* [`Linklanding plugins`](#linklanding-plugins)
* [`Linklanding plugins:install PLUGIN...`](#linklanding-pluginsinstall-plugin)
* [`Linklanding plugins:inspect PLUGIN...`](#linklanding-pluginsinspect-plugin)
* [`Linklanding plugins:install PLUGIN...`](#linklanding-pluginsinstall-plugin-1)
* [`Linklanding plugins:link PLUGIN`](#linklanding-pluginslink-plugin)
* [`Linklanding plugins:uninstall PLUGIN...`](#linklanding-pluginsuninstall-plugin)
* [`Linklanding plugins:uninstall PLUGIN...`](#linklanding-pluginsuninstall-plugin-1)
* [`Linklanding plugins:uninstall PLUGIN...`](#linklanding-pluginsuninstall-plugin-2)
* [`Linklanding plugins update`](#linklanding-plugins-update)

## `Linklanding hello PERSON`

Say hello

```
USAGE
  $ Linklanding hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Whom is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/RebootLabs-xyz/Linklanding-CLI/blob/v0.0.0/dist/commands/hello/index.ts)_

## `Linklanding hello world`

Say hello world

```
USAGE
  $ Linklanding hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oex hello world
  hello world! (./src/commands/hello/world.ts)
```

## `Linklanding help [COMMAND]`

Display help for Linklanding.

```
USAGE
  $ Linklanding help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for Linklanding.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.12/src/commands/help.ts)_

## `Linklanding plugins`

List installed plugins.

```
USAGE
  $ Linklanding plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ Linklanding plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `Linklanding plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ Linklanding plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ Linklanding plugins add

EXAMPLES
  $ Linklanding plugins:install myplugin 

  $ Linklanding plugins:install https://github.com/someuser/someplugin

  $ Linklanding plugins:install someuser/someplugin
```

## `Linklanding plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ Linklanding plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ Linklanding plugins:inspect myplugin
```

## `Linklanding plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ Linklanding plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ Linklanding plugins add

EXAMPLES
  $ Linklanding plugins:install myplugin 

  $ Linklanding plugins:install https://github.com/someuser/someplugin

  $ Linklanding plugins:install someuser/someplugin
```

## `Linklanding plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ Linklanding plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ Linklanding plugins:link myplugin
```

## `Linklanding plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ Linklanding plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ Linklanding plugins unlink
  $ Linklanding plugins remove
```

## `Linklanding plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ Linklanding plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ Linklanding plugins unlink
  $ Linklanding plugins remove
```

## `Linklanding plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ Linklanding plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ Linklanding plugins unlink
  $ Linklanding plugins remove
```

## `Linklanding plugins update`

Update installed plugins.

```
USAGE
  $ Linklanding plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
