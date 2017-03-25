# api documentation for  [commander (v2.9.0)](https://github.com/tj/commander.js#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-commander.svg)](https://travis-ci.org/npmdoc/node-npmdoc-commander)
#### the complete solution for node.js command-line programs

[![NPM](https://nodei.co/npm/commander.png?downloads=true)](https://www.npmjs.com/package/commander)

[![apidoc](https://npmdoc.github.io/node-npmdoc-commander/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-commander_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-commander/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-commander/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk",
        "email": "tj@vision-media.ca"
    },
    "bugs": {
        "url": "https://github.com/tj/commander.js/issues"
    },
    "dependencies": {
        "graceful-readlink": ">= 1.0.0"
    },
    "description": "the complete solution for node.js command-line programs",
    "devDependencies": {
        "should": ">= 0.0.1",
        "sinon": ">=1.17.1"
    },
    "directories": {},
    "dist": {
        "shasum": "9c99094176e12240cb22d6c5146098400fe0f7d4",
        "tarball": "https://registry.npmjs.org/commander/-/commander-2.9.0.tgz"
    },
    "engines": {
        "node": ">= 0.6.x"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "b2aad7a8471d434593a85306aa73777a526e9f75",
    "homepage": "https://github.com/tj/commander.js#readme",
    "keywords": [
        "command",
        "option",
        "parser"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "tjholowaychuk",
            "email": "tj@vision-media.ca"
        },
        {
            "name": "somekittens",
            "email": "rkoutnik@gmail.com"
        },
        {
            "name": "zhiyelee",
            "email": "zhiyelee@gmail.com"
        }
    ],
    "name": "commander",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tj/commander.js.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "2.9.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module commander](#apidoc.module.commander)
1.  boolean <span class="apidocSignatureSpan">commander.</span>_allowUnknownOption
1.  [function <span class="apidocSignatureSpan">commander.</span>Command (name)](#apidoc.element.commander.Command)
1.  [function <span class="apidocSignatureSpan">commander.</span>Option (flags, description)](#apidoc.element.commander.Option)
1.  object <span class="apidocSignatureSpan">commander.</span>Command.prototype
1.  object <span class="apidocSignatureSpan">commander.</span>Option.prototype
1.  object <span class="apidocSignatureSpan">commander.</span>_args
1.  object <span class="apidocSignatureSpan">commander.</span>_execs
1.  object <span class="apidocSignatureSpan">commander.</span>commands
1.  object <span class="apidocSignatureSpan">commander.</span>options
1.  string <span class="apidocSignatureSpan">commander.</span>_name

#### [module commander.Command](#apidoc.module.commander.Command)
1.  [function <span class="apidocSignatureSpan">commander.</span>Command (name)](#apidoc.element.commander.Command.Command)

#### [module commander.Command.prototype](#apidoc.module.commander.Command.prototype)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>action (fn)](#apidoc.element.commander.Command.prototype.action)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>addImplicitHelpCommand ()](#apidoc.element.commander.Command.prototype.addImplicitHelpCommand)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>alias (alias)](#apidoc.element.commander.Command.prototype.alias)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>allowUnknownOption (arg)](#apidoc.element.commander.Command.prototype.allowUnknownOption)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>arguments (desc)](#apidoc.element.commander.Command.prototype.arguments)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>command (name, desc, opts)](#apidoc.element.commander.Command.prototype.command)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>commandHelp ()](#apidoc.element.commander.Command.prototype.commandHelp)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>description (str)](#apidoc.element.commander.Command.prototype.description)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>executeSubCommand (argv, args, unknown)](#apidoc.element.commander.Command.prototype.executeSubCommand)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>help (cb)](#apidoc.element.commander.Command.prototype.help)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>helpInformation ()](#apidoc.element.commander.Command.prototype.helpInformation)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>largestOptionLength ()](#apidoc.element.commander.Command.prototype.largestOptionLength)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>missingArgument (name)](#apidoc.element.commander.Command.prototype.missingArgument)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>name ()](#apidoc.element.commander.Command.prototype.name)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>normalize (args)](#apidoc.element.commander.Command.prototype.normalize)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>option (flags, description, fn, defaultValue)](#apidoc.element.commander.Command.prototype.option)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>optionFor (arg)](#apidoc.element.commander.Command.prototype.optionFor)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>optionHelp ()](#apidoc.element.commander.Command.prototype.optionHelp)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>optionMissingArgument (option, flag)](#apidoc.element.commander.Command.prototype.optionMissingArgument)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>opts ()](#apidoc.element.commander.Command.prototype.opts)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>outputHelp (cb)](#apidoc.element.commander.Command.prototype.outputHelp)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parse (argv)](#apidoc.element.commander.Command.prototype.parse)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parseArgs (args, unknown)](#apidoc.element.commander.Command.prototype.parseArgs)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parseExpectedArgs (args)](#apidoc.element.commander.Command.prototype.parseExpectedArgs)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parseOptions (argv)](#apidoc.element.commander.Command.prototype.parseOptions)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>unknownOption (flag)](#apidoc.element.commander.Command.prototype.unknownOption)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>usage (str)](#apidoc.element.commander.Command.prototype.usage)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>variadicArgNotLast (name)](#apidoc.element.commander.Command.prototype.variadicArgNotLast)
1.  [function <span class="apidocSignatureSpan">commander.Command.prototype.</span>version (str, flags)](#apidoc.element.commander.Command.prototype.version)

#### [module commander.Option](#apidoc.module.commander.Option)
1.  [function <span class="apidocSignatureSpan">commander.</span>Option (flags, description)](#apidoc.element.commander.Option.Option)

#### [module commander.Option.prototype](#apidoc.module.commander.Option.prototype)
1.  [function <span class="apidocSignatureSpan">commander.Option.prototype.</span>is (arg)](#apidoc.element.commander.Option.prototype.is)
1.  [function <span class="apidocSignatureSpan">commander.Option.prototype.</span>name ()](#apidoc.element.commander.Option.prototype.name)



# <a name="apidoc.module.commander"></a>[module commander](#apidoc.module.commander)

#### <a name="apidoc.element.commander.Command"></a>[function <span class="apidocSignatureSpan">commander.</span>Command (name)](#apidoc.element.commander.Command)
- description and source-code
```javascript
function Command(name) {
  this.commands = [];
  this.options = [];
  this._execs = {};
  this._allowUnknownOption = false;
  this._args = [];
  this._name = name || '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.commander.Option"></a>[function <span class="apidocSignatureSpan">commander.</span>Option (flags, description)](#apidoc.element.commander.Option)
- description and source-code
```javascript
function Option(flags, description) {
  this.flags = flags;
  this.required = ~flags.indexOf('<');
  this.optional = ~flags.indexOf('[');
  this.bool = !~flags.indexOf('-no-');
  flags = flags.split(/[ ,|]+/);
  if (flags.length > 1 && !/^[[<]/.test(flags[1])) this.short = flags.shift();
  this.long = flags.shift();
  this.description = description || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.commander.Command"></a>[module commander.Command](#apidoc.module.commander.Command)

#### <a name="apidoc.element.commander.Command.Command"></a>[function <span class="apidocSignatureSpan">commander.</span>Command (name)](#apidoc.element.commander.Command.Command)
- description and source-code
```javascript
function Command(name) {
  this.commands = [];
  this.options = [];
  this._execs = {};
  this._allowUnknownOption = false;
  this._args = [];
  this._name = name || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.commander.Command.prototype"></a>[module commander.Command.prototype](#apidoc.module.commander.Command.prototype)

#### <a name="apidoc.element.commander.Command.prototype.action"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>action (fn)](#apidoc.element.commander.Command.prototype.action)
- description and source-code
```javascript
action = function (fn) {
  var self = this;
  var listener = function(args, unknown) {
    // Parse any so-far unknown options
    args = args || [];
    unknown = unknown || [];

    var parsed = self.parseOptions(unknown);

    // Output help if necessary
    outputHelpIfNecessary(self, parsed.unknown);

    // If there are still any unknown options, then we simply
    // die, unless someone asked for help, in which case we give it
    // to them, and then we die.
    if (parsed.unknown.length > 0) {
      self.unknownOption(parsed.unknown[0]);
    }

    // Leftover arguments need to be pushed back. Fixes issue #56
    if (parsed.args.length) args = parsed.args.concat(args);

    self._args.forEach(function(arg, i) {
      if (arg.required && null == args[i]) {
        self.missingArgument(arg.name);
      } else if (arg.variadic) {
        if (i !== self._args.length - 1) {
          self.variadicArgNotLast(arg.name);
        }

        args[i] = args.splice(i);
      }
    });

    // Always append ourselves to the end of the arguments,
    // to make sure we match the number of arguments the user
    // expects
    if (self._args.length) {
      args[self._args.length] = self;
    } else {
      args.push(self);
    }

    fn.apply(self, args);
  };
  var parent = this.parent || this;
  var name = parent === this ? '*' : this._name;
  parent.on(name, listener);
  if (this._alias) parent.on(this._alias, listener);
  return this;
}
```
- example usage
```shell
...
 */

var program = require('commander');

program
.version('0.0.1')
.command('rmdir <dir> [otherDirs...]')
.action(function (dir, otherDirs) {
  console.log('rmdir %s', dir);
  if (otherDirs) {
    otherDirs.forEach(function (oDir) {
      console.log('rmdir %s', oDir);
    });
  }
});
...
```

#### <a name="apidoc.element.commander.Command.prototype.addImplicitHelpCommand"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>addImplicitHelpCommand ()](#apidoc.element.commander.Command.prototype.addImplicitHelpCommand)
- description and source-code
```javascript
addImplicitHelpCommand = function () {
  this.command('help [cmd]', 'display help for [cmd]');
}
```
- example usage
```shell
...
 * @param {Array} argv
 * @return {Command} for chaining
 * @api public
 */

Command.prototype.parse = function(argv) {
// implicit help
if (this.executables) this.addImplicitHelpCommand();

// store raw args
this.rawArgs = argv;

// guess name
this._name = this._name || basename(argv[1], '.js');
...
```

#### <a name="apidoc.element.commander.Command.prototype.alias"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>alias (alias)](#apidoc.element.commander.Command.prototype.alias)
- description and source-code
```javascript
alias = function (alias) {
  if (0 == arguments.length) return this._alias;
  this._alias = alias;
  return this;
}
```
- example usage
```shell
...
  var mode = options.setup_mode || "normal";
  env = env || 'all';
  console.log('setup for %s env(s) with %s mode', env, mode);
});

program
.command('exec <cmd>')
.alias('ex')
.description('execute the given remote cmd')
.option("-e, --exec_mode <mode>", "Which exec mode to use")
.action(function(cmd, options){
  console.log('exec "%s" using %s mode', cmd, options.exec_mode);
}).on('--help', function() {
  console.log('  Examples:');
  console.log();
...
```

#### <a name="apidoc.element.commander.Command.prototype.allowUnknownOption"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>allowUnknownOption (arg)](#apidoc.element.commander.Command.prototype.allowUnknownOption)
- description and source-code
```javascript
allowUnknownOption = function (arg) {
    this._allowUnknownOption = arguments.length === 0 || arg;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.commander.Command.prototype.arguments"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>arguments (desc)](#apidoc.element.commander.Command.prototype.arguments)
- description and source-code
```javascript
arguments = function (desc) {
  return this.parseExpectedArgs(desc.split(/ +/));
}
```
- example usage
```shell
...
'''js
#!/usr/bin/env node

var program = require('../');

program
  .version('0.0.1')
  .arguments('<cmd> [env]')
  .action(function (cmd, env) {
     cmdValue = cmd;
     envValue = env;
  });

program.parse(process.argv);
...
```

#### <a name="apidoc.element.commander.Command.prototype.command"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>command (name, desc, opts)](#apidoc.element.commander.Command.prototype.command)
- description and source-code
```javascript
command = function (name, desc, opts) {
  opts = opts || {};
  var args = name.split(/ +/);
  var cmd = new Command(args.shift());

  if (desc) {
    cmd.description(desc);
    this.executables = true;
    this._execs[cmd._name] = true;
    if (opts.isDefault) this.defaultExecutable = cmd._name;
  }

  cmd._noHelp = !!opts.noHelp;
  this.commands.push(cmd);
  cmd.parseExpectedArgs(args);
  cmd.parent = this;

  if (desc) return this;
  return cmd;
}
```
- example usage
```shell
...
 * Module dependencies.
 */

var program = require('commander');

program
.version('0.0.1')
.command('rmdir <dir> [otherDirs...]')
.action(function (dir, otherDirs) {
  console.log('rmdir %s', dir);
  if (otherDirs) {
    otherDirs.forEach(function (oDir) {
      console.log('rmdir %s', oDir);
    });
  }
...
```

#### <a name="apidoc.element.commander.Command.prototype.commandHelp"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>commandHelp ()](#apidoc.element.commander.Command.prototype.commandHelp)
- description and source-code
```javascript
commandHelp = function () {
  if (!this.commands.length) return '';

  var commands = this.commands.filter(function(cmd) {
    return !cmd._noHelp;
  }).map(function(cmd) {
    var args = cmd._args.map(function(arg) {
      return humanReadableArgName(arg);
    }).join(' ');

    return [
      cmd._name
        + (cmd._alias ? '|' + cmd._alias : '')
        + (cmd.options.length ? ' [options]' : '')
        + ' ' + args
      , cmd.description()
    ];
  });

  var width = commands.reduce(function(max, command) {
    return Math.max(max, command[0].length);
  }, 0);

  return [
    ''
    , '  Commands:'
    , ''
    , commands.map(function(cmd) {
      var desc = cmd[1] ? '  ' + cmd[1] : '';
      return pad(cmd[0], width) + desc;
    }).join('\n').replace(/^/gm, '    ')
    , ''
  ].join('\n');
}
```
- example usage
```shell
...
var usage = [
  ''
  ,'  Usage: ' + cmdName + ' ' + this.usage()
  , ''
];

var cmds = [];
var commandHelp = this.commandHelp();
if (commandHelp) cmds = [commandHelp];

var options = [
  '  Options:'
  , ''
  , '' + this.optionHelp().replace(/^/gm, '    ')
  , ''
...
```

#### <a name="apidoc.element.commander.Command.prototype.description"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>description (str)](#apidoc.element.commander.Command.prototype.description)
- description and source-code
```javascript
description = function (str) {
  if (0 === arguments.length) return this._description;
  this._description = str;
  return this;
}
```
- example usage
```shell
...
.version('0.0.1')
.option('-C, --chdir <path>', 'change the working directory')
.option('-c, --config <path>', 'set config path. defaults to ./deploy.conf')
.option('-T, --no-tests', 'ignore test hook')

program
.command('setup [env]')
.description('run setup commands for all envs')
.option("-s, --setup_mode [mode]", "Which setup mode to use")
.action(function(env, options){
  var mode = options.setup_mode || "normal";
  env = env || 'all';
  console.log('setup for %s env(s) with %s mode', env, mode);
});
...
```

#### <a name="apidoc.element.commander.Command.prototype.executeSubCommand"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>executeSubCommand (argv, args, unknown)](#apidoc.element.commander.Command.prototype.executeSubCommand)
- description and source-code
```javascript
executeSubCommand = function (argv, args, unknown) {
  args = args.concat(unknown);

  if (!args.length) this.help();
  if ('help' == args[0] && 1 == args.length) this.help();

  // <cmd> --help
  if ('help' == args[0]) {
    args[0] = args[1];
    args[1] = '--help';
  }

  // executable
  var f = argv[1];
  // name of the subcommand, link 'pm-install'
  var bin = basename(f, '.js') + '-' + args[0];


  // In case of globally installed, get the base dir where executable
  //  subcommand file should be located at
  var baseDir
    , link = readlink(f);

  // when symbolink is relative path
  if (link !== f && link.charAt(0) !== '/') {
    link = path.join(dirname(f), link)
  }
  baseDir = dirname(link);

  // prefer local './<bin>' to bin in the $PATH
  var localBin = path.join(baseDir, bin);

  // whether bin file is a js script with explicit '.js' extension
  var isExplicitJS = false;
  if (exists(localBin + '.js')) {
    bin = localBin + '.js';
    isExplicitJS = true;
  } else if (exists(localBin)) {
    bin = localBin;
  }

  args = args.slice(1);

  var proc;
  if (process.platform !== 'win32') {
    if (isExplicitJS) {
      args.unshift(localBin);
      // add executable arguments to spawn
      args = (process.execArgv || []).concat(args);

      proc = spawn('node', args, { stdio: 'inherit', customFds: [0, 1, 2] });
    } else {
      proc = spawn(bin, args, { stdio: 'inherit', customFds: [0, 1, 2] });
    }
  } else {
    args.unshift(localBin);
    proc = spawn(process.execPath, args, { stdio: 'inherit'});
  }

  proc.on('close', process.exit.bind(process));
  proc.on('error', function(err) {
    if (err.code == "ENOENT") {
      console.error('\n  %s(1) does not exist, try --help\n', bin);
    } else if (err.code == "EACCES") {
      console.error('\n  %s(1) not executable. try chmod or run with root\n', bin);
    }
    process.exit(1);
  });

  // Store the reference to the child process
  this.runningCommand = proc;
}
```
- example usage
```shell
...
var args = this.args = parsed.args;

var result = this.parseArgs(this.args, parsed.unknown);

// executable sub-commands
var name = result.args[0];
if (this._execs[name] && typeof this._execs[name] != "function") {
  return this.executeSubCommand(argv, args, parsed.unknown);
} else if (this.defaultExecutable) {
  // use the default subcommand
  args.unshift(name = this.defaultExecutable);
  return this.executeSubCommand(argv, args, parsed.unknown);
}

return result;
...
```

#### <a name="apidoc.element.commander.Command.prototype.help"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>help (cb)](#apidoc.element.commander.Command.prototype.help)
- description and source-code
```javascript
help = function (cb) {
  this.outputHelp(cb);
  process.exit();
}
```
- example usage
```shell
...
  }

function make_red(txt) {
  return colors.red(txt); //display the help text in red on the console
}
'''

## .help(cb)

  Output help information and exit immediately.
  Optional callback cb allows post-processing of help text before it is displayed.

## Examples

'''js
...
```

#### <a name="apidoc.element.commander.Command.prototype.helpInformation"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>helpInformation ()](#apidoc.element.commander.Command.prototype.helpInformation)
- description and source-code
```javascript
helpInformation = function () {
  var desc = [];
  if (this._description) {
    desc = [
      '  ' + this._description
      , ''
    ];
  }

  var cmdName = this._name;
  if (this._alias) {
    cmdName = cmdName + '|' + this._alias;
  }
  var usage = [
    ''
    ,'  Usage: ' + cmdName + ' ' + this.usage()
    , ''
  ];

  var cmds = [];
  var commandHelp = this.commandHelp();
  if (commandHelp) cmds = [commandHelp];

  var options = [
    '  Options:'
    , ''
    , '' + this.optionHelp().replace(/^/gm, '    ')
    , ''
    , ''
  ];

  return usage
    .concat(cmds)
    .concat(desc)
    .concat(options)
    .join('\n');
}
```
- example usage
```shell
...

Command.prototype.outputHelp = function(cb) {
 if (!cb) {
   cb = function(passthru) {
     return passthru;
   }
 }
 process.stdout.write(cb(this.helpInformation()));
 this.emit('--help');
};

/**
* Output help information and exit.
*
* @api public
...
```

#### <a name="apidoc.element.commander.Command.prototype.largestOptionLength"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>largestOptionLength ()](#apidoc.element.commander.Command.prototype.largestOptionLength)
- description and source-code
```javascript
largestOptionLength = function () {
  return this.options.reduce(function(max, option) {
    return Math.max(max, option.flags.length);
  }, 0);
}
```
- example usage
```shell
...
 * Return help for options.
 *
 * @return {String}
 * @api private
 */

Command.prototype.optionHelp = function() {
var width = this.largestOptionLength();

// Prepend the help information
return [pad('-h, --help', width) + '  ' + 'output usage information']
    .concat(this.options.map(function(option) {
      return pad(option.flags, width) + '  ' + option.description;
    }))
    .join('\n');
...
```

#### <a name="apidoc.element.commander.Command.prototype.missingArgument"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>missingArgument (name)](#apidoc.element.commander.Command.prototype.missingArgument)
- description and source-code
```javascript
missingArgument = function (name) {
  console.error();
  console.error("  error: missing required argument '%s'", name);
  console.error();
  process.exit(1);
}
```
- example usage
```shell
...
    }

    // Leftover arguments need to be pushed back. Fixes issue #56
    if (parsed.args.length) args = parsed.args.concat(args);

    self._args.forEach(function(arg, i) {
if (arg.required && null == args[i]) {
  self.missingArgument(arg.name);
} else if (arg.variadic) {
  if (i !== self._args.length - 1) {
    self.variadicArgNotLast(arg.name);
  }

  args[i] = args.splice(i);
}
...
```

#### <a name="apidoc.element.commander.Command.prototype.name"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>name ()](#apidoc.element.commander.Command.prototype.name)
- description and source-code
```javascript
name = function () {
  return this._name;
}
```
- example usage
```shell
...
 * @return {Command} for chaining
 * @api public
 */

Command.prototype.option = function(flags, description, fn, defaultValue) {
var self = this
  , option = new Option(flags, description)
  , oname = option.name()
  , name = camelcase(oname);

// default as 3rd arg
if (typeof fn != 'function') {
  if (fn instanceof RegExp) {
    var regex = fn;
    fn = function(val, def) {
...
```

#### <a name="apidoc.element.commander.Command.prototype.normalize"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>normalize (args)](#apidoc.element.commander.Command.prototype.normalize)
- description and source-code
```javascript
normalize = function (args) {
  var ret = []
    , arg
    , lastOpt
    , index;

  for (var i = 0, len = args.length; i < len; ++i) {
    arg = args[i];
    if (i > 0) {
      lastOpt = this.optionFor(args[i-1]);
    }

    if (arg === '--') {
      // Honor option terminator
      ret = ret.concat(args.slice(i));
      break;
    } else if (lastOpt && lastOpt.required) {
      ret.push(arg);
    } else if (arg.length > 1 && '-' == arg[0] && '-' != arg[1]) {
      arg.slice(1).split('').forEach(function(c) {
        ret.push('-' + c);
      });
    } else if (/^--/.test(arg) && ~(index = arg.indexOf('='))) {
      ret.push(arg.slice(0, index), arg.slice(index + 1));
    } else {
      ret.push(arg);
    }
  }

  return ret;
}
```
- example usage
```shell
...
// github-style sub-commands with no sub-command
if (this.executables && argv.length < 3 && !this.defaultExecutable) {
  // this user needs help
  argv.push('--help');
}

// process argv
var parsed = this.parseOptions(this.normalize(argv.slice(2)));
var args = this.args = parsed.args;

var result = this.parseArgs(this.args, parsed.unknown);

// executable sub-commands
var name = result.args[0];
if (this._execs[name] && typeof this._execs[name] != "function") {
...
```

#### <a name="apidoc.element.commander.Command.prototype.option"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>option (flags, description, fn, defaultValue)](#apidoc.element.commander.Command.prototype.option)
- description and source-code
```javascript
option = function (flags, description, fn, defaultValue) {
  var self = this
    , option = new Option(flags, description)
    , oname = option.name()
    , name = camelcase(oname);

  // default as 3rd arg
  if (typeof fn != 'function') {
    if (fn instanceof RegExp) {
      var regex = fn;
      fn = function(val, def) {
        var m = regex.exec(val);
        return m ? m[0] : def;
      }
    }
    else {
      defaultValue = fn;
      fn = null;
    }
  }

  // preassign default value only for --no-*, [optional], or <required>
  if (false == option.bool || option.optional || option.required) {
    // when --no-* we make sure default is true
    if (false == option.bool) defaultValue = true;
    // preassign only if we have a default
    if (undefined !== defaultValue) self[name] = defaultValue;
  }

  // register the option
  this.options.push(option);

  // when it's passed assign the value
  // and conditionally invoke the callback
  this.on(oname, function(val) {
    // coercion
    if (null !== val && fn) val = fn(val, undefined === self[name]
      ? defaultValue
      : self[name]);

    // unassigned or bool
    if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
      // if no value, bool true, and we have a default, then use it!
      if (null == val) {
        self[name] = option.bool
          ? defaultValue || true
          : false;
      } else {
        self[name] = val;
      }
    } else if (null !== val) {
      // reassign
      self[name] = val;
    }
  });

  return this;
}
```
- example usage
```shell
...

## Installation

   $ npm install commander

## Option parsing

Options with commander are defined with the '.option()' method, also serving as documentation for the options. The example below
 parses args and options from 'process.argv', leaving remaining args as the 'program.args' array which were not consumed by options
.

'''js
#!/usr/bin/env node

/**
* Module dependencies.
*/
...
```

#### <a name="apidoc.element.commander.Command.prototype.optionFor"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>optionFor (arg)](#apidoc.element.commander.Command.prototype.optionFor)
- description and source-code
```javascript
optionFor = function (arg) {
  for (var i = 0, len = this.options.length; i < len; ++i) {
    if (this.options[i].is(arg)) {
      return this.options[i];
    }
  }
}
```
- example usage
```shell
...
, arg
, lastOpt
, index;

  for (var i = 0, len = args.length; i < len; ++i) {
arg = args[i];
if (i > 0) {
  lastOpt = this.optionFor(args[i-1]);
}

if (arg === '--') {
  // Honor option terminator
  ret = ret.concat(args.slice(i));
  break;
} else if (lastOpt && lastOpt.required) {
...
```

#### <a name="apidoc.element.commander.Command.prototype.optionHelp"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>optionHelp ()](#apidoc.element.commander.Command.prototype.optionHelp)
- description and source-code
```javascript
optionHelp = function () {
  var width = this.largestOptionLength();

  // Prepend the help information
  return [pad('-h, --help', width) + '  ' + 'output usage information']
      .concat(this.options.map(function(option) {
        return pad(option.flags, width) + '  ' + option.description;
      }))
      .join('\n');
}
```
- example usage
```shell
...
var cmds = [];
var commandHelp = this.commandHelp();
if (commandHelp) cmds = [commandHelp];

var options = [
  '  Options:'
  , ''
  , '' + this.optionHelp().replace(/^/gm, '    ')
  , ''
  , ''
];

return usage
  .concat(cmds)
  .concat(desc)
...
```

#### <a name="apidoc.element.commander.Command.prototype.optionMissingArgument"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>optionMissingArgument (option, flag)](#apidoc.element.commander.Command.prototype.optionMissingArgument)
- description and source-code
```javascript
optionMissingArgument = function (option, flag) {
  console.error();
  if (flag) {
    console.error("  error: option '%s' argument missing, got '%s'", option.flags, flag);
  } else {
    console.error("  error: option '%s' argument missing", option.flags);
  }
  console.error();
  process.exit(1);
}
```
- example usage
```shell
...
option = this.optionFor(arg);

// option is defined
if (option) {
  // requires arg
  if (option.required) {
    arg = argv[++i];
    if (null == arg) return this.optionMissingArgument(option);
    this.emit(option.name(), arg);
  // optional arg
  } else if (option.optional) {
    arg = argv[i+1];
    if (null == arg || ('-' == arg[0] && '-' != arg)) {
      arg = null;
    } else {
...
```

#### <a name="apidoc.element.commander.Command.prototype.opts"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>opts ()](#apidoc.element.commander.Command.prototype.opts)
- description and source-code
```javascript
opts = function () {
  var result = {}
    , len = this.options.length;

  for (var i = 0 ; i < len; i++) {
    var key = camelcase(this.options[i].name());
    result[key] = key === 'version' ? this._version : this[key];
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.commander.Command.prototype.outputHelp"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>outputHelp (cb)](#apidoc.element.commander.Command.prototype.outputHelp)
- description and source-code
```javascript
outputHelp = function (cb) {
  if (!cb) {
    cb = function(passthru) {
      return passthru;
    }
  }
  process.stdout.write(cb(this.helpInformation()));
  this.emit('--help');
}
```
- example usage
```shell
...
Examples:

  $ custom-help --help
  $ custom-help -h

'''

## .outputHelp(cb)

Output help information without exiting.
Optional callback cb allows post-processing of help text before it is displayed.

If you want to display help by default (e.g. if no command was provided), you can use something like:

'''js
...
```

#### <a name="apidoc.element.commander.Command.prototype.parse"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parse (argv)](#apidoc.element.commander.Command.prototype.parse)
- description and source-code
```javascript
parse = function (argv) {
  // implicit help
  if (this.executables) this.addImplicitHelpCommand();

  // store raw args
  this.rawArgs = argv;

  // guess name
  this._name = this._name || basename(argv[1], '.js');

  // github-style sub-commands with no sub-command
  if (this.executables && argv.length < 3 && !this.defaultExecutable) {
    // this user needs help
    argv.push('--help');
  }

  // process argv
  var parsed = this.parseOptions(this.normalize(argv.slice(2)));
  var args = this.args = parsed.args;

  var result = this.parseArgs(this.args, parsed.unknown);

  // executable sub-commands
  var name = result.args[0];
  if (this._execs[name] && typeof this._execs[name] != "function") {
    return this.executeSubCommand(argv, args, parsed.unknown);
  } else if (this.defaultExecutable) {
    // use the default subcommand
    args.unshift(name = this.defaultExecutable);
    return this.executeSubCommand(argv, args, parsed.unknown);
  }

  return result;
}
```
- example usage
```shell
...

program
  .version('0.0.1')
  .option('-p, --peppers', 'Add peppers')
  .option('-P, --pineapple', 'Add pineapple')
  .option('-b, --bbq-sauce', 'Add bbq sauce')
  .option('-c, --cheese [type]', 'Add the specified type of cheese [marble]', 'marble')
  .parse(process.argv);

console.log('you ordered a pizza with:');
if (program.peppers) console.log('  - peppers');
if (program.pineapple) console.log('  - pineapple');
if (program.bbqSauce) console.log('  - bbq');
console.log('  - %s cheese', program.cheese);
'''
...
```

#### <a name="apidoc.element.commander.Command.prototype.parseArgs"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parseArgs (args, unknown)](#apidoc.element.commander.Command.prototype.parseArgs)
- description and source-code
```javascript
parseArgs = function (args, unknown) {
  var name;

  if (args.length) {
    name = args[0];
    if (this.listeners(name).length) {
      this.emit(args.shift(), args, unknown);
    } else {
      this.emit('*', args);
    }
  } else {
    outputHelpIfNecessary(this, unknown);

    // If there were no args and we have unknown options,
    // then they are extraneous and we need to error.
    if (unknown.length > 0) {
      this.unknownOption(unknown[0]);
    }
  }

  return this;
}
```
- example usage
```shell
...
  argv.push('--help');
}

// process argv
var parsed = this.parseOptions(this.normalize(argv.slice(2)));
var args = this.args = parsed.args;

var result = this.parseArgs(this.args, parsed.unknown);

// executable sub-commands
var name = result.args[0];
if (this._execs[name] && typeof this._execs[name] != "function") {
  return this.executeSubCommand(argv, args, parsed.unknown);
} else if (this.defaultExecutable) {
  // use the default subcommand
...
```

#### <a name="apidoc.element.commander.Command.prototype.parseExpectedArgs"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parseExpectedArgs (args)](#apidoc.element.commander.Command.prototype.parseExpectedArgs)
- description and source-code
```javascript
parseExpectedArgs = function (args) {
  if (!args.length) return;
  var self = this;
  args.forEach(function(arg) {
    var argDetails = {
      required: false,
      name: '',
      variadic: false
    };

    switch (arg[0]) {
      case '<':
        argDetails.required = true;
        argDetails.name = arg.slice(1, -1);
        break;
      case '[':
        argDetails.name = arg.slice(1, -1);
        break;
    }

    if (argDetails.name.length > 3 && argDetails.name.slice(-3) === '...') {
      argDetails.variadic = true;
      argDetails.name = argDetails.name.slice(0, -3);
    }
    if (argDetails.name) {
      self._args.push(argDetails);
    }
  });
  return this;
}
```
- example usage
```shell
...
    this.executables = true;
    this._execs[cmd._name] = true;
    if (opts.isDefault) this.defaultExecutable = cmd._name;
  }

  cmd._noHelp = !!opts.noHelp;
  this.commands.push(cmd);
  cmd.parseExpectedArgs(args);
  cmd.parent = this;

  if (desc) return this;
  return cmd;
};

/**
...
```

#### <a name="apidoc.element.commander.Command.prototype.parseOptions"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>parseOptions (argv)](#apidoc.element.commander.Command.prototype.parseOptions)
- description and source-code
```javascript
parseOptions = function (argv) {
  var args = []
    , len = argv.length
    , literal
    , option
    , arg;

  var unknownOptions = [];

  // parse options
  for (var i = 0; i < len; ++i) {
    arg = argv[i];

    // literal args after --
    if ('--' == arg) {
      literal = true;
      continue;
    }

    if (literal) {
      args.push(arg);
      continue;
    }

    // find matching Option
    option = this.optionFor(arg);

    // option is defined
    if (option) {
      // requires arg
      if (option.required) {
        arg = argv[++i];
        if (null == arg) return this.optionMissingArgument(option);
        this.emit(option.name(), arg);
      // optional arg
      } else if (option.optional) {
        arg = argv[i+1];
        if (null == arg || ('-' == arg[0] && '-' != arg)) {
          arg = null;
        } else {
          ++i;
        }
        this.emit(option.name(), arg);
      // bool
      } else {
        this.emit(option.name());
      }
      continue;
    }

    // looks like an option
    if (arg.length > 1 && '-' == arg[0]) {
      unknownOptions.push(arg);

      // If the next argument looks like it might be
      // an argument for this option, we pass it on.
      // If it isn't, then it'll simply be ignored
      if (argv[i+1] && '-' != argv[i+1][0]) {
        unknownOptions.push(argv[++i]);
      }
      continue;
    }

    // arg
    args.push(arg);
  }

  return { args: args, unknown: unknownOptions };
}
```
- example usage
```shell
...
Command.prototype.action = function(fn) {
  var self = this;
  var listener = function(args, unknown) {
// Parse any so-far unknown options
args = args || [];
unknown = unknown || [];

var parsed = self.parseOptions(unknown);

// Output help if necessary
outputHelpIfNecessary(self, parsed.unknown);

// If there are still any unknown options, then we simply
// die, unless someone asked for help, in which case we give it
// to them, and then we die.
...
```

#### <a name="apidoc.element.commander.Command.prototype.unknownOption"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>unknownOption (flag)](#apidoc.element.commander.Command.prototype.unknownOption)
- description and source-code
```javascript
unknownOption = function (flag) {
  if (this._allowUnknownOption) return;
  console.error();
  console.error("  error: unknown option '%s'", flag);
  console.error();
  process.exit(1);
}
```
- example usage
```shell
...
// Output help if necessary
outputHelpIfNecessary(self, parsed.unknown);

// If there are still any unknown options, then we simply
// die, unless someone asked for help, in which case we give it
// to them, and then we die.
if (parsed.unknown.length > 0) {
  self.unknownOption(parsed.unknown[0]);
}

// Leftover arguments need to be pushed back. Fixes issue #56
if (parsed.args.length) args = parsed.args.concat(args);

self._args.forEach(function(arg, i) {
  if (arg.required && null == args[i]) {
...
```

#### <a name="apidoc.element.commander.Command.prototype.usage"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>usage (str)](#apidoc.element.commander.Command.prototype.usage)
- description and source-code
```javascript
usage = function (str) {
  var args = this._args.map(function(arg) {
    return humanReadableArgName(arg);
  });

  var usage = '[options]'
    + (this.commands.length ? ' [command]' : '')
    + (this._args.length ? ' ' + args.join(' ') : '');

  if (0 == arguments.length) return this._usage || usage;
  this._usage = str;

  return this;
}
```
- example usage
```shell
...

function increaseVerbosity(v, total) {
return total + 1;
}

program
.version('0.0.1')
.usage('[options] <file ...>')
.option('-i, --integer <n>', 'An integer argument', parseInt)
.option('-f, --float <n>', 'A float argument', parseFloat)
.option('-r, --range <a>..<b>', 'A range', range)
.option('-l, --list <items>', 'A list', list)
.option('-o, --optional [value]', 'An optional value')
.option('-c, --collect [value]', 'A repeatable value', collect, [])
.option('-v, --verbose', 'A value that can be increased', increaseVerbosity, 0)
...
```

#### <a name="apidoc.element.commander.Command.prototype.variadicArgNotLast"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>variadicArgNotLast (name)](#apidoc.element.commander.Command.prototype.variadicArgNotLast)
- description and source-code
```javascript
variadicArgNotLast = function (name) {
  console.error();
  console.error("  error: variadic arguments must be last '%s'", name);
  console.error();
  process.exit(1);
}
```
- example usage
```shell
...
if (parsed.args.length) args = parsed.args.concat(args);

self._args.forEach(function(arg, i) {
  if (arg.required && null == args[i]) {
    self.missingArgument(arg.name);
  } else if (arg.variadic) {
    if (i !== self._args.length - 1) {
      self.variadicArgNotLast(arg.name);
    }

    args[i] = args.splice(i);
  }
});

// Always append ourselves to the end of the arguments,
...
```

#### <a name="apidoc.element.commander.Command.prototype.version"></a>[function <span class="apidocSignatureSpan">commander.Command.prototype.</span>version (str, flags)](#apidoc.element.commander.Command.prototype.version)
- description and source-code
```javascript
version = function (str, flags) {
  if (0 == arguments.length) return this._version;
  this._version = str;
  flags = flags || '-V, --version';
  this.option(flags, 'output the version number');
  this.on('version', function() {
    process.stdout.write(str + '\n');
    process.exit(0);
  });
  return this;
}
```
- example usage
```shell
...
/**
 * Module dependencies.
 */

var program = require('commander');

program
  .version('0.0.1')
  .option('-p, --peppers', 'Add peppers')
  .option('-P, --pineapple', 'Add pineapple')
  .option('-b, --bbq-sauce', 'Add bbq sauce')
  .option('-c, --cheese [type]', 'Add the specified type of cheese [marble]', 'marble')
  .parse(process.argv);

console.log('you ordered a pizza with:');
...
```



# <a name="apidoc.module.commander.Option"></a>[module commander.Option](#apidoc.module.commander.Option)

#### <a name="apidoc.element.commander.Option.Option"></a>[function <span class="apidocSignatureSpan">commander.</span>Option (flags, description)](#apidoc.element.commander.Option.Option)
- description and source-code
```javascript
function Option(flags, description) {
  this.flags = flags;
  this.required = ~flags.indexOf('<');
  this.optional = ~flags.indexOf('[');
  this.bool = !~flags.indexOf('-no-');
  flags = flags.split(/[ ,|]+/);
  if (flags.length > 1 && !/^[[<]/.test(flags[1])) this.short = flags.shift();
  this.long = flags.shift();
  this.description = description || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.commander.Option.prototype"></a>[module commander.Option.prototype](#apidoc.module.commander.Option.prototype)

#### <a name="apidoc.element.commander.Option.prototype.is"></a>[function <span class="apidocSignatureSpan">commander.Option.prototype.</span>is (arg)](#apidoc.element.commander.Option.prototype.is)
- description and source-code
```javascript
is = function (arg) {
  return arg == this.short || arg == this.long;
}
```
- example usage
```shell
...
* @param {String} arg
* @return {Option}
* @api private
*/

Command.prototype.optionFor = function(arg) {
 for (var i = 0, len = this.options.length; i < len; ++i) {
   if (this.options[i].is(arg)) {
     return this.options[i];
   }
 }
};

/**
* Parse options from 'argv' returning 'argv'
...
```

#### <a name="apidoc.element.commander.Option.prototype.name"></a>[function <span class="apidocSignatureSpan">commander.Option.prototype.</span>name ()](#apidoc.element.commander.Option.prototype.name)
- description and source-code
```javascript
name = function () {
  return this.long
    .replace('--', '')
    .replace('no-', '');
}
```
- example usage
```shell
...
 * @return {Command} for chaining
 * @api public
 */

Command.prototype.option = function(flags, description, fn, defaultValue) {
var self = this
  , option = new Option(flags, description)
  , oname = option.name()
  , name = camelcase(oname);

// default as 3rd arg
if (typeof fn != 'function') {
  if (fn instanceof RegExp) {
    var regex = fn;
    fn = function(val, def) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
