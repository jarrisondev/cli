oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @afordin/cli
$ afordin COMMAND
running command...
$ afordin (--version)
@afordin/cli/0.1.0-beta.1 win32-x64 node-v18.16.0
$ afordin --help [COMMAND]
USAGE
  $ afordin COMMAND
...
```
<!-- usagestop -->
```sh-session
$ npm install -g @afordin/cli
$ afordin COMMAND
running command...
$ afordin (--version)
@afordin/cli/0.1.0-beta.0 win32-x64 node-v18.16.0
$ afordin --help [COMMAND]
USAGE
  $ afordin COMMAND
...
```
<!-- usagestop -->
```sh-session
$ npm install -g oclif-hello-world
$ oex COMMAND
running command...
$ oex (--version)
oclif-hello-world/0.0.0 darwin-x64 node-v16.13.1
$ oex --help [COMMAND]
USAGE
  $ oex COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`afordin create`](#afordin-create)
* [`afordin hello PERSON`](#afordin-hello-person)
* [`afordin hello:world`](#afordin-helloworld)
* [`afordin help [COMMANDS]`](#afordin-help-commands)
* [`afordin plugins`](#afordin-plugins)
* [`afordin plugins:install PLUGIN...`](#afordin-pluginsinstall-plugin)
* [`afordin plugins:inspect PLUGIN...`](#afordin-pluginsinspect-plugin)
* [`afordin plugins:install PLUGIN...`](#afordin-pluginsinstall-plugin-1)
* [`afordin plugins:link PLUGIN`](#afordin-pluginslink-plugin)
* [`afordin plugins:uninstall PLUGIN...`](#afordin-pluginsuninstall-plugin)
* [`afordin plugins:reset`](#afordin-pluginsreset)
* [`afordin plugins:uninstall PLUGIN...`](#afordin-pluginsuninstall-plugin-1)
* [`afordin plugins:uninstall PLUGIN...`](#afordin-pluginsuninstall-plugin-2)
* [`afordin plugins:update`](#afordin-pluginsupdate)

## `afordin create`

Create scaffolding projects

```
USAGE
  $ afordin create

DESCRIPTION
  Create scaffolding projects
```

_See code: [dist/commands/create/index.ts](https://github.com/afordin/cli/blob/v0.1.0-beta.1/dist/commands/create/index.ts)_

## `afordin hello PERSON`

Say hello

```
USAGE
  $ afordin hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/afordin/cli/blob/v0.1.0-beta.1/dist/commands/hello/index.ts)_

## `afordin hello:world`

Say hello world

```
USAGE
  $ afordin hello:world

DESCRIPTION
  Say hello world

EXAMPLES
  $ afordin hello:world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [dist/commands/hello/world.ts](https://github.com/afordin/cli/blob/v0.1.0-beta.1/dist/commands/hello/world.ts)_

## `afordin help [COMMANDS]`

Display help for afordin.

```
USAGE
  $ afordin help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for afordin.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.20/lib/commands/help.ts)_

## `afordin plugins`

List installed plugins.

```
USAGE
  $ afordin plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ afordin plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/index.ts)_

## `afordin plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ afordin plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -s, --silent   Silences yarn output.
  -v, --verbose  Show verbose yarn output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ afordin plugins:add

EXAMPLES
  $ afordin plugins:add myplugin 

  $ afordin plugins:add https://github.com/someuser/someplugin

  $ afordin plugins:add someuser/someplugin
```

## `afordin plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ afordin plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ afordin plugins:inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/inspect.ts)_

## `afordin plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ afordin plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -s, --silent   Silences yarn output.
  -v, --verbose  Show verbose yarn output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ afordin plugins:add

EXAMPLES
  $ afordin plugins:install myplugin 

  $ afordin plugins:install https://github.com/someuser/someplugin

  $ afordin plugins:install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/install.ts)_

## `afordin plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ afordin plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ afordin plugins:link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/link.ts)_

## `afordin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ afordin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ afordin plugins:unlink
  $ afordin plugins:remove

EXAMPLES
  $ afordin plugins:remove myplugin
```

## `afordin plugins:reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ afordin plugins:reset
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/reset.ts)_

## `afordin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ afordin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ afordin plugins:unlink
  $ afordin plugins:remove

EXAMPLES
  $ afordin plugins:uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/uninstall.ts)_

## `afordin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ afordin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ afordin plugins:unlink
  $ afordin plugins:remove

EXAMPLES
  $ afordin plugins:unlink myplugin
```

## `afordin plugins:update`

Update installed plugins.

```
USAGE
  $ afordin plugins:update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/update.ts)_
<!-- commandsstop -->
* [`afordin help [COMMANDS]`](#afordin-help-commands)
* [`afordin plugins`](#afordin-plugins)
* [`afordin plugins:install PLUGIN...`](#afordin-pluginsinstall-plugin)
* [`afordin plugins:inspect PLUGIN...`](#afordin-pluginsinspect-plugin)
* [`afordin plugins:install PLUGIN...`](#afordin-pluginsinstall-plugin-1)
* [`afordin plugins:link PLUGIN`](#afordin-pluginslink-plugin)
* [`afordin plugins:uninstall PLUGIN...`](#afordin-pluginsuninstall-plugin)
* [`afordin plugins:reset`](#afordin-pluginsreset)
* [`afordin plugins:uninstall PLUGIN...`](#afordin-pluginsuninstall-plugin-1)
* [`afordin plugins:uninstall PLUGIN...`](#afordin-pluginsuninstall-plugin-2)
* [`afordin plugins:update`](#afordin-pluginsupdate)

## `afordin help [COMMANDS]`

Display help for afordin.

```
USAGE
  $ afordin help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for afordin.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.20/lib/commands/help.ts)_

## `afordin plugins`

List installed plugins.

```
USAGE
  $ afordin plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ afordin plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/index.ts)_

## `afordin plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ afordin plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -s, --silent   Silences yarn output.
  -v, --verbose  Show verbose yarn output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ afordin plugins:add

EXAMPLES
  $ afordin plugins:add myplugin 

  $ afordin plugins:add https://github.com/someuser/someplugin

  $ afordin plugins:add someuser/someplugin
```

## `afordin plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ afordin plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ afordin plugins:inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/inspect.ts)_

## `afordin plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ afordin plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -s, --silent   Silences yarn output.
  -v, --verbose  Show verbose yarn output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ afordin plugins:add

EXAMPLES
  $ afordin plugins:install myplugin 

  $ afordin plugins:install https://github.com/someuser/someplugin

  $ afordin plugins:install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/install.ts)_

## `afordin plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ afordin plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ afordin plugins:link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/link.ts)_

## `afordin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ afordin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ afordin plugins:unlink
  $ afordin plugins:remove

EXAMPLES
  $ afordin plugins:remove myplugin
```

## `afordin plugins:reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ afordin plugins:reset
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/reset.ts)_

## `afordin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ afordin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ afordin plugins:unlink
  $ afordin plugins:remove

EXAMPLES
  $ afordin plugins:uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/uninstall.ts)_

## `afordin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ afordin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ afordin plugins:unlink
  $ afordin plugins:remove

EXAMPLES
  $ afordin plugins:unlink myplugin
```

## `afordin plugins:update`

Update installed plugins.

```
USAGE
  $ afordin plugins:update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v4.1.8/lib/commands/plugins/update.ts)_
<!-- commandsstop -->
* [`oex hello PERSON`](#oex-hello-person)
* [`oex hello world`](#oex-hello-world)
* [`oex help [COMMAND]`](#oex-help-command)
* [`oex plugins`](#oex-plugins)
* [`oex plugins:inspect PLUGIN...`](#oex-pluginsinspect-plugin)
* [`oex plugins:install PLUGIN...`](#oex-pluginsinstall-plugin)
* [`oex plugins:link PLUGIN`](#oex-pluginslink-plugin)
* [`oex plugins:uninstall PLUGIN...`](#oex-pluginsuninstall-plugin)
* [`oex plugins update`](#oex-plugins-update)

## `oex hello PERSON`

Say hello

```
USAGE
  $ oex hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/oclif/hello-world/blob/v0.0.0/dist/commands/hello/index.ts)_

## `oex hello world`

Say hello world

```
USAGE
  $ oex hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oex hello world
  hello world! (./src/commands/hello/world.ts)
```

## `oex help [COMMAND]`

Display help for oex.

```
USAGE
  $ oex help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for oex.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `oex plugins`

List installed plugins.

```
USAGE
  $ oex plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ oex plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `oex plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ oex plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ oex plugins:inspect myplugin
```

## `oex plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ oex plugins:install PLUGIN...

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
  $ oex plugins add

EXAMPLES
  $ oex plugins:install myplugin 

  $ oex plugins:install https://github.com/someuser/someplugin

  $ oex plugins:install someuser/someplugin
```

## `oex plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ oex plugins:link PLUGIN

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
  $ oex plugins:link myplugin
```

## `oex plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ oex plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oex plugins unlink
  $ oex plugins remove
```

## `oex plugins update`

Update installed plugins.

```
USAGE
  $ oex plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
