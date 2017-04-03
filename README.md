# api documentation for  [forever (v0.15.3)](https://github.com/foreverjs/forever#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-forever.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-forever) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-forever.svg)](https://travis-ci.org/npmdoc/node-npmdoc-forever)
#### A simple CLI tool for ensuring that a given node script runs continuously (i.e. forever)

[![NPM](https://nodei.co/npm/forever.png?downloads=true)](https://www.npmjs.com/package/forever)

[![apidoc](https://npmdoc.github.io/node-npmdoc-forever/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-forever_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-forever/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-forever/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-forever/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "bin": {
        "forever": "./bin/forever"
    },
    "bugs": {
        "url": "https://github.com/foreverjs/forever/issues"
    },
    "dependencies": {
        "cliff": "~0.1.9",
        "clone": "^1.0.2",
        "colors": "~0.6.2",
        "flatiron": "~0.4.2",
        "forever-monitor": "~1.7.0",
        "nconf": "~0.6.9",
        "nssocket": "~0.5.1",
        "object-assign": "^3.0.0",
        "optimist": "~0.6.0",
        "path-is-absolute": "~1.0.0",
        "prettyjson": "^1.1.2",
        "shush": "^1.0.0",
        "timespan": "~2.3.0",
        "utile": "~0.2.1",
        "winston": "~0.8.1"
    },
    "description": "A simple CLI tool for ensuring that a given node script runs continuously (i.e. forever)",
    "devDependencies": {
        "broadway": "~0.3.6",
        "eventemitter2": "0.4.x",
        "request": "2.x.x",
        "vows": "0.7.x"
    },
    "directories": {},
    "dist": {
        "shasum": "77d9d7e15fd2f511ad9d84a110c7dd8fc8ecebc2",
        "tarball": "https://registry.npmjs.org/forever/-/forever-0.15.3.tgz"
    },
    "engines": {
        "node": ">= 0.8.x"
    },
    "gitHead": "3aa17a1088eb812eb03b49219e329fb4a48b4dfc",
    "homepage": "https://github.com/foreverjs/forever#readme",
    "keywords": [
        "cli",
        "fault tolerant",
        "sysadmin",
        "tools"
    ],
    "license": "MIT",
    "main": "./lib/forever",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "bradleymeck",
            "email": "bradley.meck@gmail.com"
        },
        {
            "name": "julianduque",
            "email": "julianduquej@gmail.com"
        },
        {
            "name": "jeffsu",
            "email": "me@jeffsu.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        }
    ],
    "name": "forever",
    "optionalDependencies": {},
    "preferGlobal": "true",
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/foreverjs/forever.git"
    },
    "scripts": {
        "test": "vows test/**/*-test.js --spec -i"
    },
    "version": "0.15.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module forever](#apidoc.module.forever)
1.  boolean <span class="apidocSignatureSpan">forever.</span>initialized
1.  [function <span class="apidocSignatureSpan">forever.</span>Forever (script, options)](#apidoc.element.forever.Forever)
1.  [function <span class="apidocSignatureSpan">forever.</span>Monitor (script, options)](#apidoc.element.forever.Monitor)
1.  [function <span class="apidocSignatureSpan">forever.</span>Monitor.super_ (options)](#apidoc.element.forever.Monitor.super_)
1.  [function <span class="apidocSignatureSpan">forever.</span>Worker (options)](#apidoc.element.forever.Worker)
1.  [function <span class="apidocSignatureSpan">forever.</span>_debug ()](#apidoc.element.forever._debug)
1.  [function <span class="apidocSignatureSpan">forever.</span>checkProcess (pid)](#apidoc.element.forever.checkProcess)
1.  [function <span class="apidocSignatureSpan">forever.</span>cleanLogsSync (processes)](#apidoc.element.forever.cleanLogsSync)
1.  [function <span class="apidocSignatureSpan">forever.</span>cleanUp (cleanLogs, allowManager)](#apidoc.element.forever.cleanUp)
1.  [function <span class="apidocSignatureSpan">forever.</span>findById (id, processes)](#apidoc.element.forever.findById)
1.  [function <span class="apidocSignatureSpan">forever.</span>findByIndex (index, processes)](#apidoc.element.forever.findByIndex)
1.  [function <span class="apidocSignatureSpan">forever.</span>findByPid (pid, processes)](#apidoc.element.forever.findByPid)
1.  [function <span class="apidocSignatureSpan">forever.</span>findByScript (script, processes)](#apidoc.element.forever.findByScript)
1.  [function <span class="apidocSignatureSpan">forever.</span>findByUid (script, processes)](#apidoc.element.forever.findByUid)
1.  [function <span class="apidocSignatureSpan">forever.</span>format (format, procs)](#apidoc.element.forever.format)
1.  [function <span class="apidocSignatureSpan">forever.</span>kill (pid, killTree, signal, callback)](#apidoc.element.forever.kill)
1.  [function <span class="apidocSignatureSpan">forever.</span>list (format, callback)](#apidoc.element.forever.list)
1.  [function <span class="apidocSignatureSpan">forever.</span>load (options)](#apidoc.element.forever.load)
1.  [function <span class="apidocSignatureSpan">forever.</span>logEvents (monitor)](#apidoc.element.forever.logEvents)
1.  [function <span class="apidocSignatureSpan">forever.</span>logFilePath (logFile, uid)](#apidoc.element.forever.logFilePath)
1.  [function <span class="apidocSignatureSpan">forever.</span>pidFilePath (pidFile)](#apidoc.element.forever.pidFilePath)
1.  [function <span class="apidocSignatureSpan">forever.</span>restart (target, format)](#apidoc.element.forever.restart)
1.  [function <span class="apidocSignatureSpan">forever.</span>restartAll (format)](#apidoc.element.forever.restartAll)
1.  [function <span class="apidocSignatureSpan">forever.</span>start (script, options)](#apidoc.element.forever.start)
1.  [function <span class="apidocSignatureSpan">forever.</span>startDaemon (script, options)](#apidoc.element.forever.startDaemon)
1.  [function <span class="apidocSignatureSpan">forever.</span>startServer ()](#apidoc.element.forever.startServer)
1.  [function <span class="apidocSignatureSpan">forever.</span>stat (logFile, script, callback)](#apidoc.element.forever.stat)
1.  [function <span class="apidocSignatureSpan">forever.</span>stop (target, format)](#apidoc.element.forever.stop)
1.  [function <span class="apidocSignatureSpan">forever.</span>stopAll (format)](#apidoc.element.forever.stopAll)
1.  [function <span class="apidocSignatureSpan">forever.</span>stopbypid (pid, format)](#apidoc.element.forever.stopbypid)
1.  [function <span class="apidocSignatureSpan">forever.</span>tail (target, options, callback)](#apidoc.element.forever.tail)
1.  object <span class="apidocSignatureSpan">forever.</span>Monitor.prototype
1.  object <span class="apidocSignatureSpan">forever.</span>Monitor.super_.prototype
1.  object <span class="apidocSignatureSpan">forever.</span>Monitor.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">forever.</span>Worker.prototype
1.  object <span class="apidocSignatureSpan">forever.</span>cli
1.  object <span class="apidocSignatureSpan">forever.</span>columns
1.  object <span class="apidocSignatureSpan">forever.</span>config
1.  object <span class="apidocSignatureSpan">forever.</span>log
1.  object <span class="apidocSignatureSpan">forever.</span>out
1.  string <span class="apidocSignatureSpan">forever.</span>root
1.  string <span class="apidocSignatureSpan">forever.</span>version

#### [module forever.Monitor](#apidoc.module.forever.Monitor)
1.  [function <span class="apidocSignatureSpan">forever.</span>Monitor (script, options)](#apidoc.element.forever.Monitor.Monitor)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.</span>parseCommand (command, args)](#apidoc.element.forever.Monitor.parseCommand)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.</span>super_ (options)](#apidoc.element.forever.Monitor.super_)

#### [module forever.Monitor.prototype](#apidoc.module.forever.Monitor.prototype)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>_getEnv ()](#apidoc.element.forever.Monitor.prototype._getEnv)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>kill (forceStop)](#apidoc.element.forever.Monitor.prototype.kill)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>restart ()](#apidoc.element.forever.Monitor.prototype.restart)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>send (msg)](#apidoc.element.forever.Monitor.prototype.send)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>start (restart)](#apidoc.element.forever.Monitor.prototype.start)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>stop ()](#apidoc.element.forever.Monitor.prototype.stop)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>toString ()](#apidoc.element.forever.Monitor.prototype.toString)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>trySpawn ()](#apidoc.element.forever.Monitor.prototype.trySpawn)
1.  object <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>inspect

#### [module forever.Monitor.super_](#apidoc.module.forever.Monitor.super_)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.</span>super_ (conf)](#apidoc.element.forever.Monitor.super_.super_)

#### [module forever.Monitor.super_.prototype](#apidoc.module.forever.Monitor.super_.prototype)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>init (options, callback)](#apidoc.element.forever.Monitor.super_.prototype.init)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>inspect ()](#apidoc.element.forever.Monitor.super_.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>remove (name)](#apidoc.element.forever.Monitor.super_.prototype.remove)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>use (plugin, options, callback)](#apidoc.element.forever.Monitor.super_.prototype.use)

#### [module forever.Monitor.super_.super_.prototype](#apidoc.module.forever.Monitor.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>addListener (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>emit ()](#apidoc.element.forever.Monitor.super_.super_.prototype.emit)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>listeners (type)](#apidoc.element.forever.Monitor.super_.super_.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>listenersAny ()](#apidoc.element.forever.Monitor.super_.super_.prototype.listenersAny)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>many (event, ttl, fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.many)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>off (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.off)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>offAny (fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.offAny)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>on (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>onAny (fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.onAny)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>once (event, fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.once)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>removeAllListeners (type)](#apidoc.element.forever.Monitor.super_.super_.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>removeListener (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>setMaxListeners (n)](#apidoc.element.forever.Monitor.super_.super_.prototype.setMaxListeners)
1.  string <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>delimiter
1.  string <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>event

#### [module forever.Worker](#apidoc.module.forever.Worker)
1.  [function <span class="apidocSignatureSpan">forever.</span>Worker (options)](#apidoc.element.forever.Worker.Worker)
1.  [function <span class="apidocSignatureSpan">forever.Worker.</span>super_ ()](#apidoc.element.forever.Worker.super_)

#### [module forever.Worker.prototype](#apidoc.module.forever.Worker.prototype)
1.  [function <span class="apidocSignatureSpan">forever.Worker.prototype.</span>start (callback)](#apidoc.element.forever.Worker.prototype.start)

#### [module forever.cli](#apidoc.module.forever.cli)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>addColumn (name)](#apidoc.element.forever.cli.addColumn)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>cleanLogs ()](#apidoc.element.forever.cli.cleanLogs)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>clear (key)](#apidoc.element.forever.cli.clear)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>config ()](#apidoc.element.forever.cli.config)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>getOptions (file)](#apidoc.element.forever.cli.getOptions)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>help ()](#apidoc.element.forever.cli.help)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>list ()](#apidoc.element.forever.cli.list)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>logFiles (index)](#apidoc.element.forever.cli.logFiles)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>logs (index)](#apidoc.element.forever.cli.logs)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>resetColumns ()](#apidoc.element.forever.cli.resetColumns)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>restart (file)](#apidoc.element.forever.cli.restart)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>restartAll ()](#apidoc.element.forever.cli.restartAll)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>rmColumn (name)](#apidoc.element.forever.cli.rmColumn)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>run ()](#apidoc.element.forever.cli.run)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>set (key, value)](#apidoc.element.forever.cli.set)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>setColumns (columns)](#apidoc.element.forever.cli.setColumns)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>start ()](#apidoc.element.forever.cli.start)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>startDaemon ()](#apidoc.element.forever.cli.startDaemon)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>stop (file)](#apidoc.element.forever.cli.stop)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>stopall ()](#apidoc.element.forever.cli.stopall)
1.  [function <span class="apidocSignatureSpan">forever.cli.</span>stopbypid (pid)](#apidoc.element.forever.cli.stopbypid)
1.  object <span class="apidocSignatureSpan">forever.cli.</span>argvOptions

#### [module forever.log](#apidoc.module.forever.log)
1.  boolean <span class="apidocSignatureSpan">forever.log.</span>emitErrs
1.  boolean <span class="apidocSignatureSpan">forever.log.</span>exitOnError
1.  boolean <span class="apidocSignatureSpan">forever.log.</span>padLevels
1.  boolean <span class="apidocSignatureSpan">forever.log.</span>stripColors
1.  [function <span class="apidocSignatureSpan">forever.log.</span>data (msg)](#apidoc.element.forever.log.data)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>debug (msg)](#apidoc.element.forever.log.debug)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>error (msg)](#apidoc.element.forever.log.error)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>help (msg)](#apidoc.element.forever.log.help)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>info (msg)](#apidoc.element.forever.log.info)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>input (msg)](#apidoc.element.forever.log.input)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>prompt (msg)](#apidoc.element.forever.log.prompt)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>silly (msg)](#apidoc.element.forever.log.silly)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>verbose (msg)](#apidoc.element.forever.log.verbose)
1.  [function <span class="apidocSignatureSpan">forever.log.</span>warn (msg)](#apidoc.element.forever.log.warn)
1.  number <span class="apidocSignatureSpan">forever.log.</span>_eventsCount
1.  number <span class="apidocSignatureSpan">forever.log.</span>levelLength
1.  object <span class="apidocSignatureSpan">forever.log.</span>_events
1.  object <span class="apidocSignatureSpan">forever.log.</span>_hnames
1.  object <span class="apidocSignatureSpan">forever.log.</span>_names
1.  object <span class="apidocSignatureSpan">forever.log.</span>domain
1.  object <span class="apidocSignatureSpan">forever.log.</span>exceptionHandlers
1.  object <span class="apidocSignatureSpan">forever.log.</span>levels
1.  object <span class="apidocSignatureSpan">forever.log.</span>profilers
1.  object <span class="apidocSignatureSpan">forever.log.</span>rewriters
1.  object <span class="apidocSignatureSpan">forever.log.</span>transports
1.  string <span class="apidocSignatureSpan">forever.log.</span>level

#### [module forever.out](#apidoc.module.forever.out)
1.  boolean <span class="apidocSignatureSpan">forever.out.</span>emitErrs
1.  boolean <span class="apidocSignatureSpan">forever.out.</span>exitOnError
1.  boolean <span class="apidocSignatureSpan">forever.out.</span>padLevels
1.  boolean <span class="apidocSignatureSpan">forever.out.</span>stripColors
1.  [function <span class="apidocSignatureSpan">forever.out.</span>debug (msg)](#apidoc.element.forever.out.debug)
1.  [function <span class="apidocSignatureSpan">forever.out.</span>error (msg)](#apidoc.element.forever.out.error)
1.  [function <span class="apidocSignatureSpan">forever.out.</span>info (msg)](#apidoc.element.forever.out.info)
1.  [function <span class="apidocSignatureSpan">forever.out.</span>silly (msg)](#apidoc.element.forever.out.silly)
1.  [function <span class="apidocSignatureSpan">forever.out.</span>verbose (msg)](#apidoc.element.forever.out.verbose)
1.  [function <span class="apidocSignatureSpan">forever.out.</span>warn (msg)](#apidoc.element.forever.out.warn)
1.  number <span class="apidocSignatureSpan">forever.out.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">forever.out.</span>_events
1.  object <span class="apidocSignatureSpan">forever.out.</span>_hnames
1.  object <span class="apidocSignatureSpan">forever.out.</span>_names
1.  object <span class="apidocSignatureSpan">forever.out.</span>domain
1.  object <span class="apidocSignatureSpan">forever.out.</span>exceptionHandlers
1.  object <span class="apidocSignatureSpan">forever.out.</span>levels
1.  object <span class="apidocSignatureSpan">forever.out.</span>profilers
1.  object <span class="apidocSignatureSpan">forever.out.</span>rewriters
1.  object <span class="apidocSignatureSpan">forever.out.</span>transports
1.  string <span class="apidocSignatureSpan">forever.out.</span>level



# <a name="apidoc.module.forever"></a>[module forever](#apidoc.module.forever)

#### <a name="apidoc.element.forever.Forever"></a>[function <span class="apidocSignatureSpan">forever.</span>Forever (script, options)](#apidoc.element.forever.Forever)
- description and source-code
```javascript
Forever = function (script, options) {
  //
  // Simple bootstrapper for attaching logger
  // and watch plugins by default. Other plugins
  // can be attached through 'monitor.use(plugin, options)'.
  //
  function bootstrap(monitor) {
    plugins.logger.attach.call(monitor, options);
    if (options.watch) {
      plugins.watch.attach.call(monitor, options);
    }
  }

  var execPath = process.execPath,
      self     = this;

  //
  // Setup basic configuration options
  //
  options               = options || {};
  this.silent           = options.silent || false;
  this.killTree         = options.killTree !== false;
  this.uid              = options.uid || utile.randomString(4);
  this.id               = options.id || false;
  this.pidFile          = options.pidFile;
  this.max              = options.max;
  this.killTTL          = options.killTTL;
  this.killSignal       = options.killSignal || 'SIGKILL';
  this.childExists      = false;
  this.checkFile        = options.checkFile !== false;
  this.times            = 0;
  this.warn             = console.error;

  this.logFile          = options.logFile;
  this.outFile          = options.outFile;
  this.errFile          = options.errFile;
  this.append           = options.append;
  this.usePolling       = options.usePolling;
  this.pollingInterval  = options.pollingInterval;

  //
  // Define some safety checks for commands with spaces
  //
  this.parser = options.parser || Monitor.parseCommand;

  //
  // Setup restart timing. These options control how quickly forever restarts
  // a child process as well as when to kill a "spinning" process
  //
  this.minUptime     = typeof options.minUptime !== 'number' ? 0 : options.minUptime;
  this.spinSleepTime = options.spinSleepTime || null;

  //
  // Special case Windows separately to decouple any
  // future changes
  //
  if (process.platform === 'win32') {
    execPath = '"' + execPath + '"';
  }

  if (options.options) {
    console.warn('options.options is deprecated. Use options.args instead.');
  }

  //
  // Setup the command to spawn and the options to pass
  // to that command.
  //
  this.command   = options.command || execPath;
  this.args      = options.args || options.options || [];
  this.spawnWith = options.spawnWith || {};
  this.sourceDir = options.sourceDir;
  this.fork      = options.fork || false;
  this.cwd       = options.cwd || process.cwd();
  this.hideEnv   = options.hideEnv || [];
  this._env      = options.env || {};
  this._hideEnv  = {};

  //
  // Allow for custom stdio configuration of forked processes
  //
  this.stdio = options.stdio || null;

  //
  // Setup watch configuration options
  //
  this.watchIgnoreDotFiles = options.watchIgnoreDotFiles !== false;
  this.watchIgnorePatterns = options.watchIgnorePatterns || [];
  this.watchDirectory      = options.watchDirectory || this.sourceDir;

  //
  // Create a simple mapping of 'this.hideEnv' to an easily indexable
  // object
  //
  this.hideEnv.forEach(function (key) {
    self._hideEnv[key] = true;
  });

  if (Array.isArray(script)) {
    this.command = script[0];
    this.args = script.slice(1);
  }
  else {
    this.args.unshift(script);
  }

  if (this.sourceDir) {
    this.args[0] = path.join(this.sourceDir, this.args[0]);
  }

  //
  // Bootstrap this instance now that options
  // have been set
  //
  broadway.App.call(this, { bootstrapper: { bootstrap: bootstrap } });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor"></a>[function <span class="apidocSignatureSpan">forever.</span>Monitor (script, options)](#apidoc.element.forever.Monitor)
- description and source-code
```javascript
Monitor = function (script, options) {
  //
  // Simple bootstrapper for attaching logger
  // and watch plugins by default. Other plugins
  // can be attached through 'monitor.use(plugin, options)'.
  //
  function bootstrap(monitor) {
    plugins.logger.attach.call(monitor, options);
    if (options.watch) {
      plugins.watch.attach.call(monitor, options);
    }
  }

  var execPath = process.execPath,
      self     = this;

  //
  // Setup basic configuration options
  //
  options               = options || {};
  this.silent           = options.silent || false;
  this.killTree         = options.killTree !== false;
  this.uid              = options.uid || utile.randomString(4);
  this.id               = options.id || false;
  this.pidFile          = options.pidFile;
  this.max              = options.max;
  this.killTTL          = options.killTTL;
  this.killSignal       = options.killSignal || 'SIGKILL';
  this.childExists      = false;
  this.checkFile        = options.checkFile !== false;
  this.times            = 0;
  this.warn             = console.error;

  this.logFile          = options.logFile;
  this.outFile          = options.outFile;
  this.errFile          = options.errFile;
  this.append           = options.append;
  this.usePolling       = options.usePolling;
  this.pollingInterval  = options.pollingInterval;

  //
  // Define some safety checks for commands with spaces
  //
  this.parser = options.parser || Monitor.parseCommand;

  //
  // Setup restart timing. These options control how quickly forever restarts
  // a child process as well as when to kill a "spinning" process
  //
  this.minUptime     = typeof options.minUptime !== 'number' ? 0 : options.minUptime;
  this.spinSleepTime = options.spinSleepTime || null;

  //
  // Special case Windows separately to decouple any
  // future changes
  //
  if (process.platform === 'win32') {
    execPath = '"' + execPath + '"';
  }

  if (options.options) {
    console.warn('options.options is deprecated. Use options.args instead.');
  }

  //
  // Setup the command to spawn and the options to pass
  // to that command.
  //
  this.command   = options.command || execPath;
  this.args      = options.args || options.options || [];
  this.spawnWith = options.spawnWith || {};
  this.sourceDir = options.sourceDir;
  this.fork      = options.fork || false;
  this.cwd       = options.cwd || process.cwd();
  this.hideEnv   = options.hideEnv || [];
  this._env      = options.env || {};
  this._hideEnv  = {};

  //
  // Allow for custom stdio configuration of forked processes
  //
  this.stdio = options.stdio || null;

  //
  // Setup watch configuration options
  //
  this.watchIgnoreDotFiles = options.watchIgnoreDotFiles !== false;
  this.watchIgnorePatterns = options.watchIgnorePatterns || [];
  this.watchDirectory      = options.watchDirectory || this.sourceDir;

  //
  // Create a simple mapping of 'this.hideEnv' to an easily indexable
  // object
  //
  this.hideEnv.forEach(function (key) {
    self._hideEnv[key] = true;
  });

  if (Array.isArray(script)) {
    this.command = script[0];
    this.args = script.slice(1);
  }
  else {
    this.args.unshift(script);
  }

  if (this.sourceDir) {
    this.args[0] = path.join(this.sourceDir, this.args[0]);
  }

  //
  // Bootstrap this instance now that options
  // have been set
  //
  broadway.App.call(this, { bootstrapper: { bootstrap: bootstrap } });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_"></a>[function <span class="apidocSignatureSpan">forever.</span>Monitor.super_ (options)](#apidoc.element.forever.Monitor.super_)
- description and source-code
```javascript
Monitor.super_ = function (options) {
  //
  // Setup options and 'App' constants.
  //
  options        = options || {};
  this.root      = options.root;
  this.delimiter = options.delimiter || '::';

  //
  // Inherit from 'EventEmitter2'
  //
  events.EventEmitter2.call(this, {
    delimiter: this.delimiter,
    wildcard: true
  });

  //
  // Setup other relevant options such as the plugins
  // for this instance.
  //
  this.options      = options;
  this.env          = options.env || process.env['NODE_ENV'] || 'development'
  this.plugins      = options.plugins || {};
  this.initialized  = false;
  this.bootstrapper = options.bootstrapper || bootstrapper;
  this.initializers = {};
  this.initlist     = [];

  //
  // Bootstrap this instance
  //
  this.bootstrapper.bootstrap(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Worker"></a>[function <span class="apidocSignatureSpan">forever.</span>Worker (options)](#apidoc.element.forever.Worker)
- description and source-code
```javascript
Worker = function (options) {
  events.EventEmitter.call(this);
  options = options || {};

  this.monitor  = options.monitor;
  this.sockPath = options.sockPath || forever.config.get('sockPath');
  this.exitOnStop = options.exitOnStop === true;

  this._socket = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever._debug"></a>[function <span class="apidocSignatureSpan">forever.</span>_debug ()](#apidoc.element.forever._debug)
- description and source-code
```javascript
_debug = function () {
  var debug = forever.config.get('debug');

  if (!debug) {
    forever.config.set('debug', true);
    forever.log.add(winston.transports.File, {
      level: 'silly',
      filename: path.join(forever.config.get('root'), 'forever.debug.log')
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.checkProcess"></a>[function <span class="apidocSignatureSpan">forever.</span>checkProcess (pid)](#apidoc.element.forever.checkProcess)
- description and source-code
```javascript
checkProcess = function (pid) {
  if (!pid) {
    return false;
  }

  try {
    //
    // Trying to kill non-existent process here raises a ESRCH - no such
    // process exception. Also, signal 0 doesn't do no harm to a process - it
    // only checks if sending a signal to a given process is possible.
    //
    process.kill(pid, 0);
    return true;
  }
  catch (err) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cleanLogsSync"></a>[function <span class="apidocSignatureSpan">forever.</span>cleanLogsSync (processes)](#apidoc.element.forever.cleanLogsSync)
- description and source-code
```javascript
cleanLogsSync = function (processes) {
  var root = forever.config.get('root'),
      files = fs.readdirSync(root),
      running,
      runningLogs;

  running = processes && processes.filter(function (p) {
    return p && p.logFile;
  });

  runningLogs = running && running.map(function (p) {
    return p.logFile.split('/').pop();
  });

  files.forEach(function (file) {
    if (/\.log$/.test(file) && (!runningLogs || runningLogs.indexOf(file) === -1)) {
      fs.unlinkSync(path.join(root, file));
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cleanUp"></a>[function <span class="apidocSignatureSpan">forever.</span>cleanUp (cleanLogs, allowManager)](#apidoc.element.forever.cleanUp)
- description and source-code
```javascript
cleanUp = function (cleanLogs, allowManager) {
  var emitter = new events.EventEmitter(),
      pidPath = forever.config.get('pidPath');

  getAllProcesses(function (err, processes) {
    if (err) {
      return process.nextTick(function () {
        emitter.emit('error', err);
      });
    }
    else if (cleanLogs) {
      forever.cleanLogsSync(processes);
    }

    function unlinkProcess(proc, done) {
      fs.unlink(path.join(pidPath, proc.uid + '.pid'), function () {
        //
        // Ignore errors (in case the file doesnt exist).
        //

        if (cleanLogs && proc.logFile) {
          //
          // If we are cleaning logs then do so if the process
          // has a logfile.
          //
          return fs.unlink(proc.logFile, function () {
            done();
          });
        }

        done();
      });
    }

    function cleanProcess(proc, done) {
      if (proc.child && proc.manager) {
        return done();
      }
      else if (!proc.child && !proc.manager
        || (!proc.child && proc.manager && allowManager)
        || proc.dead) {
        return unlinkProcess(proc, done);
      }

      //
      // If we have a manager but no child, wait a moment
      // in-case the child is currently restarting, but **only**
      // if we have not already waited for this process
      //
      if (!proc.waited) {
        proc.waited = true;
        return setTimeout(function () {
          checkProcess(proc, done);
        }, 500);
      }

      done();
    }

    function checkProcess(proc, next) {
      proc.child = forever.checkProcess(proc.pid);
      proc.manager = forever.checkProcess(proc.foreverPid);
      cleanProcess(proc, next);
    }

    if (processes && processes.length > 0) {
      (function cleanBatch(batch) {
        async.forEach(batch, checkProcess, function () {
          return processes.length > 0
            ? cleanBatch(processes.splice(0, 10))
            : emitter.emit('cleanUp');
        });
      })(processes.splice(0, 10));
    }
    else {
      process.nextTick(function () {
        emitter.emit('cleanUp');
      });
    }
  });

  return emitter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.findById"></a>[function <span class="apidocSignatureSpan">forever.</span>findById (id, processes)](#apidoc.element.forever.findById)
- description and source-code
```javascript
findById = function (id, processes) {
  if (!processes) { return null; }

  var procs = processes.filter(function (p) {
    return p.id === id;
  });

  if (procs.length === 0) { procs = null; }
  return procs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.findByIndex"></a>[function <span class="apidocSignatureSpan">forever.</span>findByIndex (index, processes)](#apidoc.element.forever.findByIndex)
- description and source-code
```javascript
findByIndex = function (index, processes) {
  var indexAsNum = parseInt(index, 10),
      proc;

  if (indexAsNum == index) {
    proc = processes && processes[indexAsNum];
  }
  return proc ? [proc] : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.findByPid"></a>[function <span class="apidocSignatureSpan">forever.</span>findByPid (pid, processes)](#apidoc.element.forever.findByPid)
- description and source-code
```javascript
findByPid = function (pid, processes) {
  pid = typeof pid === 'string'
    ? parseInt(pid, 10)
    : pid;

  var procs = processes && processes.filter(function (p) {
    return p.pid === pid;
  });

  if (procs && procs.length === 0) { procs = null; }
  return procs || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.findByScript"></a>[function <span class="apidocSignatureSpan">forever.</span>findByScript (script, processes)](#apidoc.element.forever.findByScript)
- description and source-code
```javascript
findByScript = function (script, processes) {
  if (!processes) { return null; }

  // make script absolute.
  if (script.indexOf('/') != 0) {
    script = path.resolve(process.cwd(), script);
  }

  var procs = processes.filter(function (p) {
    return p.file === script || path.join(p.spawnWith.cwd, p.file) === script;
  });

  if (procs.length === 0) { procs = null; }
  return procs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.findByUid"></a>[function <span class="apidocSignatureSpan">forever.</span>findByUid (script, processes)](#apidoc.element.forever.findByUid)
- description and source-code
```javascript
findByUid = function (script, processes) {
  var procs = !processes
    ? null
    : processes.filter(function (p) {
      return p.uid === script;
    });

  if (procs && procs.length === 0) { procs = null; }
  return procs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.format"></a>[function <span class="apidocSignatureSpan">forever.</span>format (format, procs)](#apidoc.element.forever.format)
- description and source-code
```javascript
format = function (format, procs) {
  if (!procs || procs.length === 0) {
    return null;
  }

  var index = 0,
      columns = forever.config.get('columns'),
      rows = [['   '].concat(columns)],
      formatted;

  function mapColumns(prefix, mapFn) {
    return [prefix].concat(columns.map(mapFn));
  }

  if (format) {
    //
    // Iterate over the procs to see which has the
    // longest options string
    //
    procs.forEach(function (proc) {
      rows.push(mapColumns('[' + index + ']', function (column) {
        return forever.columns[column]
          ? forever.columns[column].get(proc)
          : 'MISSING';
      }));

      index++;
    });

    formatted = cliff.stringifyRows(rows, mapColumns('white', function (column) {
      return forever.columns[column]
        ? forever.columns[column].color
        : 'white';
    }));
  }

  return format ? formatted : procs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.kill"></a>[function <span class="apidocSignatureSpan">forever.</span>kill (pid, killTree, signal, callback)](#apidoc.element.forever.kill)
- description and source-code
```javascript
kill = function (pid, killTree, signal, callback) {
  signal   = signal   || 'SIGKILL';
  callback = callback || function () {};

  if (killTree && process.platform !== 'win32') {
    psTree(pid, function (err, children) {
      [pid].concat(
        children.map(function (p) {
          return p.PID;
        })
      ).forEach(function (tpid) {
        try { process.kill(tpid, signal) }
        catch (ex) { }
      });

      callback();
    });
  }
  else {
    try { process.kill(pid, signal) }
    catch (ex) { }
    callback();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.list"></a>[function <span class="apidocSignatureSpan">forever.</span>list (format, callback)](#apidoc.element.forever.list)
- description and source-code
```javascript
list = function (format, callback) {
  getAllProcesses(function (err, processes) {
    callback(err, forever.format(format, processes));
  });
}
```
- example usage
```shell
...
  }
]
'''

### Using In Your Code
The forever module exposes some useful methods to use in your code. Each method returns an instance of an EventEmitter which emits
 when complete. See the [forever cli commands][2] for sample usage.

**Remark:** As of 'forever@0.6.0' processes will not automatically be available in 'forever.list()'. In order to get your processes
 into 'forever.list()' or 'forever list' you must instantiate the 'forever' socket server:

''' js
  forever.startServer(child);
'''

This method takes multiple 'forever.Monitor' instances which are defined in the 'forever-monitor' dependency.
...
```

#### <a name="apidoc.element.forever.load"></a>[function <span class="apidocSignatureSpan">forever.</span>load (options)](#apidoc.element.forever.load)
- description and source-code
```javascript
load = function (options) {
  // memorize current options.
  this._loadedOptions = options;

  //
  // Setup the incoming options with default options.
  //
  options           = options           || {};
  options.loglength = options.loglength || 100;
  options.logstream = options.logstream || false;
  options.root      = options.root      || forever.root;
  options.pidPath   = options.pidPath   || path.join(options.root, 'pids');
  options.sockPath  = options.sockPath  || path.join(options.root, 'sock');

  //
  // If forever is initalized and the config directories are identical
  // simply return without creating directories
  //
  if (forever.initialized && forever.config.get('root') === options.root &&
    forever.config.get('pidPath') === options.pidPath) {
    return;
  }

  forever.config = new nconf.File({ file: path.join(options.root, 'config.json') });

  //
  // Try to load the forever 'config.json' from
  // the specified location.
  //
  try {
    forever.config.loadSync();
  }
  catch (ex) { }

  //
  // Setup the columns for 'forever list'.
  //
  options.columns  = options.columns  || forever.config.get('columns');
  if (!options.columns) {
    options.columns = [
      'uid', 'command', 'script', 'forever', 'pid', 'id', 'logfile', 'uptime'
    ];
  }

  forever.config.set('root', options.root);
  forever.config.set('pidPath', options.pidPath);
  forever.config.set('sockPath', options.sockPath);
  forever.config.set('loglength', options.loglength);
  forever.config.set('logstream', options.logstream);
  forever.config.set('columns', options.columns);

  //
  // Setup timestamp to event logger
  //
  forever.out.transports.console.timestamp = forever.config.get('timestamp') === 'true';

  //
  // Attempt to see if 'forever' has been configured to
  // run in debug mode.
  //
  options.debug = options.debug || forever.config.get('debug') || false;

  if (options.debug) {
    //
    // If we have been indicated to debug this forever process
    // then setup 'forever._debug' to be an instance of 'winston.Logger'.
    //
    forever._debug();
  }

  //
  // Syncronously create the 'root' directory
  // and the 'pid' directory for forever. Although there is
  // an additional overhead here of the sync action. It simplifies
  // the setup of forever dramatically.
  //
  function tryCreate(dir) {
    try {
      fs.mkdirSync(dir, '0755');
    }
    catch (ex) { }
  }

  tryCreate(forever.config.get('root'));
  tryCreate(forever.config.get('pidPath'));
  tryCreate(forever.config.get('sockPath'));

  //
  // Attempt to save the new 'config.json' for forever
  //
  try {
    forever.config.saveSync();
  }
  catch (ex) { }

  forever.initialized = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.logEvents"></a>[function <span class="apidocSignatureSpan">forever.</span>logEvents (monitor)](#apidoc.element.forever.logEvents)
- description and source-code
```javascript
logEvents = function (monitor) {
  monitor.on('watch:error', function (info) {
    forever.out.error(info.message);
    forever.out.error(info.error);
  });

  monitor.on('watch:restart', function (info) {
    forever.out.error('restarting script because ' + info.file + ' changed');
  });

  monitor.on('restart', function () {
    forever.out.error('Script restart attempt #' + monitor.times);
  });

  monitor.on('exit:code', function (code, signal) {
    forever.out.error((code !== null && code !== undefined)
      ? 'Forever detected script exited with code: ' + code
      : 'Forever detected script was killed by signal: ' + signal);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.logFilePath"></a>[function <span class="apidocSignatureSpan">forever.</span>logFilePath (logFile, uid)](#apidoc.element.forever.logFilePath)
- description and source-code
```javascript
logFilePath = function (logFile, uid) {
  return logFile && (logFile[0] === '/' || logFile[1] === ':')
    ? logFile
    : path.join(forever.config.get('root'), logFile || (uid || 'forever') + '.log');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.pidFilePath"></a>[function <span class="apidocSignatureSpan">forever.</span>pidFilePath (pidFile)](#apidoc.element.forever.pidFilePath)
- description and source-code
```javascript
pidFilePath = function (pidFile) {
  return pidFile && (pidFile[0] === '/' || pidFile[1] === ':')
    ? pidFile
    : path.join(forever.config.get('pidPath'), pidFile);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.restart"></a>[function <span class="apidocSignatureSpan">forever.</span>restart (target, format)](#apidoc.element.forever.restart)
- description and source-code
```javascript
restart = function (target, format) {
  return stopOrRestart('restart', 'restart', format, target);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.restartAll"></a>[function <span class="apidocSignatureSpan">forever.</span>restartAll (format)](#apidoc.element.forever.restartAll)
- description and source-code
```javascript
restartAll = function (format) {
  return stopOrRestart('restart', 'restartAll', format);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.start"></a>[function <span class="apidocSignatureSpan">forever.</span>start (script, options)](#apidoc.element.forever.start)
- description and source-code
```javascript
start = function (script, options) {
  if (!options.uid) {
    options.uid = utile.randomString(4).replace(/^\-/, '_');
  }

  if (!options.logFile) {
    options.logFile = forever.logFilePath(options.uid + '.log');
  }

  //
  // Create the monitor, log events, and start.
  //
  var monitor = new forever.Monitor(script, options);
  forever.logEvents(monitor);
  return monitor.start();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.startDaemon"></a>[function <span class="apidocSignatureSpan">forever.</span>startDaemon (script, options)](#apidoc.element.forever.startDaemon)
- description and source-code
```javascript
startDaemon = function (script, options) {
  options         = options || {};
  options.uid     = options.uid || utile.randomString(4).replace(/^\-/, '_');
  options.logFile = forever.logFilePath(options.logFile || forever.config.get('logFile') || options.uid + '.log');
  options.pidFile = forever.pidFilePath(options.pidFile || forever.config.get('pidFile') || options.uid + '.pid');

  var monitor, outFD, errFD, monitorPath;

  //
  // This log file is forever's log file - the user's outFile and errFile
  // options are not taken into account here.  This will be an aggregate of all
  // the app's output, as well as messages from the monitor process, where
  // applicable.
  //
  outFD = fs.openSync(options.logFile, 'a');
  errFD = fs.openSync(options.logFile, 'a');
  monitorPath = path.resolve(__dirname, '..', 'bin', 'monitor');

  monitor = spawn(process.execPath, [monitorPath, script], {
    stdio: ['ipc', outFD, errFD],
    detached: true
  });

  monitor.on('exit', function (code) {
    console.error('Monitor died unexpectedly with exit code %d', code);
  });

  // transmit options to daemonic(child) process, keep configuration lineage.
  options._loadedOptions = this._loadedOptions;

  monitor.send(JSON.stringify(options));

  // close the ipc communication channel with the monitor
  // otherwise the corresponding events listeners will prevent
  // the exit of the current process (observed with node 0.11.9)
  monitor.disconnect();

  // make sure the monitor is unref() and does not prevent the
  // exit of the current process
  monitor.unref();

  return monitor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.startServer"></a>[function <span class="apidocSignatureSpan">forever.</span>startServer ()](#apidoc.element.forever.startServer)
- description and source-code
```javascript
startServer = function () {
  var args = Array.prototype.slice.call(arguments),
      monitors = [],
      callback;

  args.forEach(function (a) {
    if (Array.isArray(a)) {
      monitors = monitors.concat(a.filter(function (m) {
        return m instanceof forever.Monitor;
      }));
    }
    else if (a instanceof forever.Monitor) {
      monitors.push(a);
    }
    else if (typeof a === 'function') {
      callback = a;
    }
  });

  async.map(monitors, function (monitor, next) {
    var worker = new forever.Worker({
      monitor: monitor,
      sockPath: forever.config.get('sockPath'),
      exitOnStop: true
    });

    worker.start(function (err) {
      return err ? next(err) : next(null, worker);
    });
  }, callback || function () {});
}
```
- example usage
```shell
...

### Using In Your Code
The forever module exposes some useful methods to use in your code. Each method returns an instance of an EventEmitter which emits
 when complete. See the [forever cli commands][2] for sample usage.

**Remark:** As of 'forever@0.6.0' processes will not automatically be available in 'forever.list()'. In order to get your processes
 into 'forever.list()' or 'forever list' you must instantiate the 'forever' socket server:

''' js
  forever.startServer(child);
'''

This method takes multiple 'forever.Monitor' instances which are defined in the 'forever-monitor' dependency.

#### forever.load (config)
_Synchronously_ sets the specified configuration (config) for the forever module. There are two important options:
...
```

#### <a name="apidoc.element.forever.stat"></a>[function <span class="apidocSignatureSpan">forever.</span>stat (logFile, script, callback)](#apidoc.element.forever.stat)
- description and source-code
```javascript
stat = function (logFile, script, callback) {
  var logAppend;

  if (arguments.length === 4) {
    logAppend = callback;
    callback = arguments[3];
  }

  fs.stat(script, function (err, stats) {
    if (err) {
      return callback(new Error('script ' + script + ' does not exist.'));
    }

    return logAppend ? callback(null) : fs.stat(logFile, function (err, stats) {
      return !err
        ? callback(new Error('log file ' + logFile + ' exists. Use the -a or --append option to append log.'))
        : callback(null);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.stop"></a>[function <span class="apidocSignatureSpan">forever.</span>stop (target, format)](#apidoc.element.forever.stop)
- description and source-code
```javascript
stop = function (target, format) {
  return stopOrRestart('stop', 'stop', format, target);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.stopAll"></a>[function <span class="apidocSignatureSpan">forever.</span>stopAll (format)](#apidoc.element.forever.stopAll)
- description and source-code
```javascript
stopAll = function (format) {
  return stopOrRestart('stop', 'stopAll', format);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.stopbypid"></a>[function <span class="apidocSignatureSpan">forever.</span>stopbypid (pid, format)](#apidoc.element.forever.stopbypid)
- description and source-code
```javascript
stopbypid = function (pid, format) {
  // stopByPid only capable of stopping, but can't restart
  return stopOrRestart('stop', 'stopByPid', format, pid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.tail"></a>[function <span class="apidocSignatureSpan">forever.</span>tail (target, options, callback)](#apidoc.element.forever.tail)
- description and source-code
```javascript
tail = function (target, options, callback) {
  if (!callback && typeof options === 'function') {
    callback = options;
    options.length = 0;
    options.stream = false;
  }

  var that   = this,
      length = options.length || forever.config.get('loglength'),
      stream = options.stream || forever.config.get('logstream'),
      blanks = function (e, i, a) { return e !== ''; },
      title  = function (e, i, a) { return e.match(/^==>/); },
      args   = ['-n', length],
      logs;

  if (stream) { args.unshift('-f'); }

  function tailProcess(procs, next) {
    var count = 0,
        map   = {},
        tail;

    procs.forEach(function (proc) {
      args.push(proc.logFile);
      map[proc.logFile] = { pid: proc.pid, file: proc.file };
      count++;
    });

    tail = spawn('tail', args, {
      stdio: [null, 'pipe', 'pipe'],
    });

    tail.stdio[1].setEncoding('utf8');
    tail.stdio[2].setEncoding('utf8');

    tail.stdio[1].on('data', function (data) {
      var chunk = data.split('\n\n');
      chunk.forEach(function (logs) {
        var logs = logs.split('\n').filter(blanks),
            file = logs.filter(title),
            lines,
            proc;

        proc = file.length
          ? map[file[0].split(' ')[1]]
          : map[procs[0].logFile];

        lines = count !== 1
          ? logs.slice(1)
          : logs;

        lines.forEach(function (line) {
          callback(null, { file: proc.file, pid: proc.pid, line: line });
        });
      });
    });

    tail.stdio[2].on('data', function (err) {
      return callback(err);
    });
  }

  getAllProcesses(function (err, processes) {
    if (err) {
      return callback(err);
    }
    else if (!processes) {
      return callback(new Error('Cannot find forever process: ' + target));
    }

    var procs = forever.findByIndex(target, processes)
      || forever.findByScript(target, processes);

    if (!procs) {
      return callback(new Error('No logs available for process: ' + target));
    }

    tailProcess(procs, callback);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Monitor"></a>[module forever.Monitor](#apidoc.module.forever.Monitor)

#### <a name="apidoc.element.forever.Monitor.Monitor"></a>[function <span class="apidocSignatureSpan">forever.</span>Monitor (script, options)](#apidoc.element.forever.Monitor.Monitor)
- description and source-code
```javascript
Monitor = function (script, options) {
  //
  // Simple bootstrapper for attaching logger
  // and watch plugins by default. Other plugins
  // can be attached through 'monitor.use(plugin, options)'.
  //
  function bootstrap(monitor) {
    plugins.logger.attach.call(monitor, options);
    if (options.watch) {
      plugins.watch.attach.call(monitor, options);
    }
  }

  var execPath = process.execPath,
      self     = this;

  //
  // Setup basic configuration options
  //
  options               = options || {};
  this.silent           = options.silent || false;
  this.killTree         = options.killTree !== false;
  this.uid              = options.uid || utile.randomString(4);
  this.id               = options.id || false;
  this.pidFile          = options.pidFile;
  this.max              = options.max;
  this.killTTL          = options.killTTL;
  this.killSignal       = options.killSignal || 'SIGKILL';
  this.childExists      = false;
  this.checkFile        = options.checkFile !== false;
  this.times            = 0;
  this.warn             = console.error;

  this.logFile          = options.logFile;
  this.outFile          = options.outFile;
  this.errFile          = options.errFile;
  this.append           = options.append;
  this.usePolling       = options.usePolling;
  this.pollingInterval  = options.pollingInterval;

  //
  // Define some safety checks for commands with spaces
  //
  this.parser = options.parser || Monitor.parseCommand;

  //
  // Setup restart timing. These options control how quickly forever restarts
  // a child process as well as when to kill a "spinning" process
  //
  this.minUptime     = typeof options.minUptime !== 'number' ? 0 : options.minUptime;
  this.spinSleepTime = options.spinSleepTime || null;

  //
  // Special case Windows separately to decouple any
  // future changes
  //
  if (process.platform === 'win32') {
    execPath = '"' + execPath + '"';
  }

  if (options.options) {
    console.warn('options.options is deprecated. Use options.args instead.');
  }

  //
  // Setup the command to spawn and the options to pass
  // to that command.
  //
  this.command   = options.command || execPath;
  this.args      = options.args || options.options || [];
  this.spawnWith = options.spawnWith || {};
  this.sourceDir = options.sourceDir;
  this.fork      = options.fork || false;
  this.cwd       = options.cwd || process.cwd();
  this.hideEnv   = options.hideEnv || [];
  this._env      = options.env || {};
  this._hideEnv  = {};

  //
  // Allow for custom stdio configuration of forked processes
  //
  this.stdio = options.stdio || null;

  //
  // Setup watch configuration options
  //
  this.watchIgnoreDotFiles = options.watchIgnoreDotFiles !== false;
  this.watchIgnorePatterns = options.watchIgnorePatterns || [];
  this.watchDirectory      = options.watchDirectory || this.sourceDir;

  //
  // Create a simple mapping of 'this.hideEnv' to an easily indexable
  // object
  //
  this.hideEnv.forEach(function (key) {
    self._hideEnv[key] = true;
  });

  if (Array.isArray(script)) {
    this.command = script[0];
    this.args = script.slice(1);
  }
  else {
    this.args.unshift(script);
  }

  if (this.sourceDir) {
    this.args[0] = path.join(this.sourceDir, this.args[0]);
  }

  //
  // Bootstrap this instance now that options
  // have been set
  //
  broadway.App.call(this, { bootstrapper: { bootstrap: bootstrap } });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.parseCommand"></a>[function <span class="apidocSignatureSpan">forever.Monitor.</span>parseCommand (command, args)](#apidoc.element.forever.Monitor.parseCommand)
- description and source-code
```javascript
parseCommand = function (command, args) {
  var match = command.match(
    process.platform === 'win32' ? safetyChecks.windows : safetyChecks.linux
  );

  //
  // No match means it's a bad command. This is configurable
  // by passing a custom 'parser' function into the 'Monitor'
  // constructor function.
  //
  if (!match) { return false; }

  if (process.platform == 'win32') {
    command = match[1] || match[2];
    if (match[3]) {
      args = match[3].split(' ').concat(args);
    }
  } else {
    command = match[1];
    if (match[2]) {
      args = match[2].split(' ').concat(this.args);
    }
  }

  return {
    command: command,
    args:    args
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_"></a>[function <span class="apidocSignatureSpan">forever.Monitor.</span>super_ (options)](#apidoc.element.forever.Monitor.super_)
- description and source-code
```javascript
super_ = function (options) {
  //
  // Setup options and 'App' constants.
  //
  options        = options || {};
  this.root      = options.root;
  this.delimiter = options.delimiter || '::';

  //
  // Inherit from 'EventEmitter2'
  //
  events.EventEmitter2.call(this, {
    delimiter: this.delimiter,
    wildcard: true
  });

  //
  // Setup other relevant options such as the plugins
  // for this instance.
  //
  this.options      = options;
  this.env          = options.env || process.env['NODE_ENV'] || 'development'
  this.plugins      = options.plugins || {};
  this.initialized  = false;
  this.bootstrapper = options.bootstrapper || bootstrapper;
  this.initializers = {};
  this.initlist     = [];

  //
  // Bootstrap this instance
  //
  this.bootstrapper.bootstrap(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Monitor.prototype"></a>[module forever.Monitor.prototype](#apidoc.module.forever.Monitor.prototype)

#### <a name="apidoc.element.forever.Monitor.prototype._getEnv"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>_getEnv ()](#apidoc.element.forever.Monitor.prototype._getEnv)
- description and source-code
```javascript
_getEnv = function () {
  var self = this,
      merged = {};

  function addKey(key, source) {
    merged[key] = source[key];
  }

  //
  // Mixin the key:value pairs from 'process.env' and the custom
  // environment variables in 'this._env'.
  //
  Object.keys(process.env).forEach(function (key) {
    if (!self._hideEnv[key]) {
      addKey(key, process.env);
    }
  });

  Object.keys(this._env).forEach(function (key) {
    addKey(key, self._env);
  });

  return merged;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.kill"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>kill (forceStop)](#apidoc.element.forever.Monitor.prototype.kill)
- description and source-code
```javascript
kill = function (forceStop) {
  var child = this.child,
      self = this,
      timer;

  if (!child || (!this.running && !this.forceRestart)) {
    process.nextTick(function () {
      self.emit('error', new Error('Cannot stop process that is not running.'));
    });
  }
  else {
    //
    // Set an instance variable here to indicate this
    // stoppage is forced so that when 'child.on('exit', ..)'
    // fires in 'Monitor.prototype.start' we can short circuit
    // and prevent auto-restart
    //
    if (forceStop) {
      this.forceStop = true;
      //
      // If we have a time before we truly kill forcefully, set up a timer
      //
      if (this.killTTL) {
        timer = setTimeout(function () {
          common.kill(self.child.pid, self.killTree, self.killSignal || 'SIGKILL');
        }, this.killTTL);

        child.once('exit', function () {
          clearTimeout(timer);
        });
      }
    }

    child.once('exit', function () {
      self.emit('stop', self.childData);
      if (self.forceRestart && !self.running) {
        self.start(true);
      }
    });

    common.kill(this.child.pid, this.killTree, this.killSignal);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.restart"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>restart ()](#apidoc.element.forever.Monitor.prototype.restart)
- description and source-code
```javascript
restart = function () {
  this.times = this.times || 0;
  this.forceRestart = true;

  return !this.running
    ? this.start(true)
    : this.kill(false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.send"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>send (msg)](#apidoc.element.forever.Monitor.prototype.send)
- description and source-code
```javascript
send = function (msg) {
  var child = this.child,
      self = this;

  if (!child || !this.running) {
    process.nextTick(function () {
      self.emit('error', new Error('Cannot send to process that is not running.'));
    });
  }

  if (child.send) { child.send(msg) }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.start"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>start (restart)](#apidoc.element.forever.Monitor.prototype.start)
- description and source-code
```javascript
start = function (restart) {
  var self = this,
      child;

  if (this.running && !restart) {
    process.nextTick(function () {
      self.emit('error', new Error('Cannot start process that is already running.'));
    });
    return this;
  }

  child = this.trySpawn();
  if (!child) {
    process.nextTick(function () {
      self.emit('error', new Error('Target script does not exist: ' + self.args[0]));
    });
    return this;
  }

  this.ctime = Date.now();
  this.child = child;
  this.running = true;
  this.isMaster = cluster.isMaster;

  process.nextTick(function () {
    self.emit(restart ? 'restart' : 'start', self, self.data);
  });

  function onMessage(msg) {
    self.emit('message', msg);
  }

  // Re-emit messages from the child process
  this.child.on('message', onMessage);

  child.on('exit', function (code, signal) {
    var spinning = Date.now() - self.ctime < self.minUptime;
    child.removeListener('message', onMessage);
    self.emit('exit:code', code, signal);

    function letChildDie() {
      self.running = false;
      self.forceStop = false;
      self.emit('exit', self, spinning);
    }

    function restartChild() {
      self.forceRestart = false;
      process.nextTick(function () {
        self.start(true);
      });
    }

    self.times++;

    if (self.forceStop || (self.times >= self.max && !self.forceRestart)
      || (spinning && typeof self.spinSleepTime !== 'number') && !self.forceRestart) {
      letChildDie();
    }
    else if (spinning) {
      setTimeout(restartChild, self.spinSleepTime);
    }
    else {
      restartChild();
    }
  });

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.stop"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>stop ()](#apidoc.element.forever.Monitor.prototype.stop)
- description and source-code
```javascript
stop = function () {
  return this.kill(true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.toString"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>toString ()](#apidoc.element.forever.Monitor.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.prototype.trySpawn"></a>[function <span class="apidocSignatureSpan">forever.Monitor.prototype.</span>trySpawn ()](#apidoc.element.forever.Monitor.prototype.trySpawn)
- description and source-code
```javascript
trySpawn = function () {
  var run = this.parser(this.command, this.args.slice()),
      stats;

  if (/[^\w]node$/.test(this.command) && this.checkFile && !this.childExists) {
    try {
      stats = fs.statSync(this.args[0]);
      this.childExists = true;
    }
    catch (ex) {
      return false;
    }
  }

  this.spawnWith.cwd = this.spawnWith.cwd || this.cwd;
  this.spawnWith.env = this._getEnv();

  if (process.platform === 'win32') {
    this.spawnWith.detached = true;
  }

  if (this.stdio) {
    this.spawnWith.stdio = this.stdio;
  }

  if (this.fork) {
    if (!this.stdio) {
      this.spawnWith.stdio = [ 'pipe', 'pipe', 'pipe', 'ipc' ];
    }
    return spawn(run.command, run.args, this.spawnWith);
  }

  return spawn(run.command, run.args, this.spawnWith);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Monitor.super_"></a>[module forever.Monitor.super_](#apidoc.module.forever.Monitor.super_)

#### <a name="apidoc.element.forever.Monitor.super_.super_"></a>[function <span class="apidocSignatureSpan">forever.Monitor.</span>super_ (conf)](#apidoc.element.forever.Monitor.super_.super_)
- description and source-code
```javascript
function EventEmitter(conf) {
  this._events = {};
  this.newListener = false;
  configure.call(this, conf);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Monitor.super_.prototype"></a>[module forever.Monitor.super_.prototype](#apidoc.module.forever.Monitor.super_.prototype)

#### <a name="apidoc.element.forever.Monitor.super_.prototype.init"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>init (options, callback)](#apidoc.element.forever.Monitor.super_.prototype.init)
- description and source-code
```javascript
init = function (options, callback) {
  if (!callback && typeof options === 'function') {
    callback = options;
    options = {};
  }

  if (this.initialized) {
    return callback();
  }

  var self = this;
  options = options   || {};
  callback = callback || function () {};
  this.env = options.env || this.env;
  this.options = common.mixin({}, this.options, options);

  function onComplete() {
    self.initialized = true;
    self.emit('init');
    callback();
  }

  function ensureFeatures (err) {
    return err
      ? onError(err)
      : features.ensure(this, onComplete);
  }

  function initPlugin(plugin, next) {
    if (typeof self.initializers[plugin] === 'function') {
      return self.initializers[plugin].call(self, function (err) {
        if (err) {
          return next(err);
        }

        self.emit(['plugin', plugin, 'init']);
        self.initializers[plugin] = true;
        next();
      });
    }

    next();
  }

  function initPlugins() {
    async.forEach(self.initlist, initPlugin, ensureFeatures);
  }

  //
  // Emit and respond with any errors that may short
  // circuit the process.
  //
  function onError(err) {
    self.emit(['error', 'init'], err);
    callback(err);
  }

  //
  // Run the bootstrapper, initialize plugins, and
  // ensure features for this instance.
  //
  this.bootstrapper.init(this, initPlugins);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.prototype.inspect"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>inspect ()](#apidoc.element.forever.Monitor.super_.prototype.inspect)
- description and source-code
```javascript
inspect = function () {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.prototype.remove"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>remove (name)](#apidoc.element.forever.Monitor.super_.prototype.remove)
- description and source-code
```javascript
remove = function (name) {
  // if this is a plugin object set the name to the plugins name
  if (name.name) {
    name = name.name;
  }

  if (this.plugins[name] && this.plugins[name].detach) {
    this.plugins[name].detach.call(this);
  }

  delete this.plugins[name];
  delete this.options[name];
  delete this.initializers[name];

  var init = this.initlist.indexOf(name);

  if (init !== -1) {
    this.initlist.splice(1, init);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.prototype.use"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.prototype.</span>use (plugin, options, callback)](#apidoc.element.forever.Monitor.super_.prototype.use)
- description and source-code
```javascript
use = function (plugin, options, callback) {
  options = options || {};

  if (typeof plugin === 'undefined') {
    console.log('Cannot load invalid plugin!');
    return callback && callback(new Error('Invalid plugin'));
  }

  var name = plugin.name,
      self = this;

  // If the plugin doesn't have a name, use itself as an identifier for the plugins hash.
  if (!name) {
    name = common.uuid();
  }

  if (this.plugins[name]) {
    return callback && callback();
  }

  //
  // Setup state on this instance for the specified plugin
  //
  this.plugins[name] = plugin;
  this.options[name] = common.mixin({}, options, this.options[name] || {});

  //
  // Attach the specified plugin to this instance, extending
  // the 'App' with new functionality.
  //
  if (this.plugins[name].attach && options.attach !== false) {
    this.plugins[name].attach.call(this, options);
  }

  //
  // Setup the initializer only if 'options.init' is
  // not false. This allows for some plugins to be lazy-loaded
  //
  if (options.init === false) {
    return callback && callback();
  }

  if (!this.initialized) {
    this.initializers[name] = plugin.init || true;
    this.initlist.push(name);
    return callback && callback();
  }
  else if (plugin.init) {
    plugin.init.call(this, function (err) {
      var args = err
        ? [['plugin', name, 'error'], err]
        : [['plugin', name, 'init']];

      self.emit.apply(self, args);
      return callback && (err ? callback(err) : callback());
    });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Monitor.super_.super_.prototype"></a>[module forever.Monitor.super_.super_.prototype](#apidoc.module.forever.Monitor.super_.super_.prototype)

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>addListener (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (type, listener) {

  if (typeof type === 'function') {
    this.onAny(type);
    return this;
  }

  if (typeof listener !== 'function') {
    throw new Error('on only accepts instances of Function');
  }
  this._events || init.call(this);

  // To avoid recursion in the case that type == "newListeners"! Before
  // adding it to the listeners, first emit "newListeners".
  this.emit('newListener', type, listener);

  if(this.wildcard) {
    growListenerTree.call(this, type, listener);
    return this;
  }

  if (!this._events[type]) {
    // Optimize the case of one listener. Don't need the extra array object.
    this._events[type] = listener;
  }
  else if(typeof this._events[type] === 'function') {
    // Adding the second element, need to change to array.
    this._events[type] = [this._events[type], listener];
  }
  else if (isArray(this._events[type])) {
    // If we've already got an array, just append.
    this._events[type].push(listener);

    // Check for listener leak
    if (!this._events[type].warned) {

      var m = defaultMaxListeners;

      if (typeof this._events.maxListeners !== 'undefined') {
        m = this._events.maxListeners;
      }

      if (m > 0 && this._events[type].length > m) {

        this._events[type].warned = true;
        console.error('(node) warning: possible EventEmitter memory ' +
                      'leak detected. %d listeners added. ' +
                      'Use emitter.setMaxListeners() to increase limit.',
                      this._events[type].length);
        console.trace();
      }
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.emit"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>emit ()](#apidoc.element.forever.Monitor.super_.super_.prototype.emit)
- description and source-code
```javascript
emit = function () {

  this._events || init.call(this);

  var type = arguments[0];

  if (type === 'newListener' && !this.newListener) {
    if (!this._events.newListener) { return false; }
  }

  // Loop through the *_all* functions and invoke them.
  if (this._all) {
    var l = arguments.length;
    var args = new Array(l - 1);
    for (var i = 1; i < l; i++) args[i - 1] = arguments[i];
    for (i = 0, l = this._all.length; i < l; i++) {
      this.event = type;
      this._all[i].apply(this, args);
    }
  }

  // If there is no 'error' event listener then throw.
  if (type === 'error') {

    if (!this._all &&
      !this._events.error &&
      !(this.wildcard && this.listenerTree.error)) {

      if (arguments[1] instanceof Error) {
        throw arguments[1]; // Unhandled 'error' event
      } else {
        throw new Error("Uncaught, unspecified 'error' event.");
      }
      return false;
    }
  }

  var handler;

  if(this.wildcard) {
    handler = [];
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    searchListenerTree.call(this, handler, ns, this.listenerTree, 0);
  }
  else {
    handler = this._events[type];
  }

  if (typeof handler === 'function') {
    this.event = type;
    if (arguments.length === 1) {
      handler.call(this);
    }
    else if (arguments.length > 1)
      switch (arguments.length) {
        case 2:
          handler.call(this, arguments[1]);
          break;
        case 3:
          handler.call(this, arguments[1], arguments[2]);
          break;
        // slower
        default:
          var l = arguments.length;
          var args = new Array(l - 1);
          for (var i = 1; i < l; i++) args[i - 1] = arguments[i];
          handler.apply(this, args);
      }
    return true;
  }
  else if (handler) {
    var l = arguments.length;
    var args = new Array(l - 1);
    for (var i = 1; i < l; i++) args[i - 1] = arguments[i];

    var listeners = handler.slice();
    for (var i = 0, l = listeners.length; i < l; i++) {
      this.event = type;
      listeners[i].apply(this, args);
    }
    return (listeners.length > 0) || !!this._all;
  }
  else {
    return !!this._all;
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.listeners"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>listeners (type)](#apidoc.element.forever.Monitor.super_.super_.prototype.listeners)
- description and source-code
```javascript
listeners = function (type) {
  if(this.wildcard) {
    var handlers = [];
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    searchListenerTree.call(this, handlers, ns, this.listenerTree, 0);
    return handlers;
  }

  this._events || init.call(this);

  if (!this._events[type]) this._events[type] = [];
  if (!isArray(this._events[type])) {
    this._events[type] = [this._events[type]];
  }
  return this._events[type];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.listenersAny"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>listenersAny ()](#apidoc.element.forever.Monitor.super_.super_.prototype.listenersAny)
- description and source-code
```javascript
listenersAny = function () {

  if(this._all) {
    return this._all;
  }
  else {
    return [];
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.many"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>many (event, ttl, fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.many)
- description and source-code
```javascript
many = function (event, ttl, fn) {
  var self = this;

  if (typeof fn !== 'function') {
    throw new Error('many only accepts instances of Function');
  }

  function listener() {
    if (--ttl === 0) {
      self.off(event, listener);
    }
    fn.apply(this, arguments);
  }

  listener._origin = fn;

  this.on(event, listener);

  return self;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.off"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>off (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.off)
- description and source-code
```javascript
off = function (type, listener) {
  if (typeof listener !== 'function') {
    throw new Error('removeListener only takes instances of Function');
  }

  var handlers,leafs=[];

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);
  }
  else {
    // does not use listeners(), so no side effect of creating _events[type]
    if (!this._events[type]) return this;
    handlers = this._events[type];
    leafs.push({_listeners:handlers});
  }

  for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
    var leaf = leafs[iLeaf];
    handlers = leaf._listeners;
    if (isArray(handlers)) {

      var position = -1;

      for (var i = 0, length = handlers.length; i < length; i++) {
        if (handlers[i] === listener ||
          (handlers[i].listener && handlers[i].listener === listener) ||
          (handlers[i]._origin && handlers[i]._origin === listener)) {
          position = i;
          break;
        }
      }

      if (position < 0) {
        continue;
      }

      if(this.wildcard) {
        leaf._listeners.splice(position, 1);
      }
      else {
        this._events[type].splice(position, 1);
      }

      if (handlers.length === 0) {
        if(this.wildcard) {
          delete leaf._listeners;
        }
        else {
          delete this._events[type];
        }
      }
      return this;
    }
    else if (handlers === listener ||
      (handlers.listener && handlers.listener === listener) ||
      (handlers._origin && handlers._origin === listener)) {
      if(this.wildcard) {
        delete leaf._listeners;
      }
      else {
        delete this._events[type];
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.offAny"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>offAny (fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.offAny)
- description and source-code
```javascript
offAny = function (fn) {
  var i = 0, l = 0, fns;
  if (fn && this._all && this._all.length > 0) {
    fns = this._all;
    for(i = 0, l = fns.length; i < l; i++) {
      if(fn === fns[i]) {
        fns.splice(i, 1);
        return this;
      }
    }
  } else {
    this._all = [];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>on (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.on)
- description and source-code
```javascript
on = function (type, listener) {

  if (typeof type === 'function') {
    this.onAny(type);
    return this;
  }

  if (typeof listener !== 'function') {
    throw new Error('on only accepts instances of Function');
  }
  this._events || init.call(this);

  // To avoid recursion in the case that type == "newListeners"! Before
  // adding it to the listeners, first emit "newListeners".
  this.emit('newListener', type, listener);

  if(this.wildcard) {
    growListenerTree.call(this, type, listener);
    return this;
  }

  if (!this._events[type]) {
    // Optimize the case of one listener. Don't need the extra array object.
    this._events[type] = listener;
  }
  else if(typeof this._events[type] === 'function') {
    // Adding the second element, need to change to array.
    this._events[type] = [this._events[type], listener];
  }
  else if (isArray(this._events[type])) {
    // If we've already got an array, just append.
    this._events[type].push(listener);

    // Check for listener leak
    if (!this._events[type].warned) {

      var m = defaultMaxListeners;

      if (typeof this._events.maxListeners !== 'undefined') {
        m = this._events.maxListeners;
      }

      if (m > 0 && this._events[type].length > m) {

        this._events[type].warned = true;
        console.error('(node) warning: possible EventEmitter memory ' +
                      'leak detected. %d listeners added. ' +
                      'Use emitter.setMaxListeners() to increase limit.',
                      this._events[type].length);
        console.trace();
      }
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.onAny"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>onAny (fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.onAny)
- description and source-code
```javascript
onAny = function (fn) {

  if (typeof fn !== 'function') {
    throw new Error('onAny only accepts instances of Function');
  }

  if(!this._all) {
    this._all = [];
  }

  // Add the function to the event listener collection.
  this._all.push(fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.once"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>once (event, fn)](#apidoc.element.forever.Monitor.super_.super_.prototype.once)
- description and source-code
```javascript
once = function (event, fn) {
  this.many(event, 1, fn);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>removeAllListeners (type)](#apidoc.element.forever.Monitor.super_.super_.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function (type) {
  if (arguments.length === 0) {
    !this._events || init.call(this);
    return this;
  }

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    var leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);

    for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
      var leaf = leafs[iLeaf];
      leaf._listeners = null;
    }
  }
  else {
    if (!this._events[type]) return this;
    this._events[type] = null;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>removeListener (type, listener)](#apidoc.element.forever.Monitor.super_.super_.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (type, listener) {
  if (typeof listener !== 'function') {
    throw new Error('removeListener only takes instances of Function');
  }

  var handlers,leafs=[];

  if(this.wildcard) {
    var ns = typeof type === 'string' ? type.split(this.delimiter) : type.slice();
    leafs = searchListenerTree.call(this, null, ns, this.listenerTree, 0);
  }
  else {
    // does not use listeners(), so no side effect of creating _events[type]
    if (!this._events[type]) return this;
    handlers = this._events[type];
    leafs.push({_listeners:handlers});
  }

  for (var iLeaf=0; iLeaf<leafs.length; iLeaf++) {
    var leaf = leafs[iLeaf];
    handlers = leaf._listeners;
    if (isArray(handlers)) {

      var position = -1;

      for (var i = 0, length = handlers.length; i < length; i++) {
        if (handlers[i] === listener ||
          (handlers[i].listener && handlers[i].listener === listener) ||
          (handlers[i]._origin && handlers[i]._origin === listener)) {
          position = i;
          break;
        }
      }

      if (position < 0) {
        continue;
      }

      if(this.wildcard) {
        leaf._listeners.splice(position, 1);
      }
      else {
        this._events[type].splice(position, 1);
      }

      if (handlers.length === 0) {
        if(this.wildcard) {
          delete leaf._listeners;
        }
        else {
          delete this._events[type];
        }
      }
      return this;
    }
    else if (handlers === listener ||
      (handlers.listener && handlers.listener === listener) ||
      (handlers._origin && handlers._origin === listener)) {
      if(this.wildcard) {
        delete leaf._listeners;
      }
      else {
        delete this._events[type];
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Monitor.super_.super_.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">forever.Monitor.super_.super_.prototype.</span>setMaxListeners (n)](#apidoc.element.forever.Monitor.super_.super_.prototype.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function (n) {
  this._events || init.call(this);
  this._events.maxListeners = n;
  if (!this._conf) this._conf = {};
  this._conf.maxListeners = n;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Worker"></a>[module forever.Worker](#apidoc.module.forever.Worker)

#### <a name="apidoc.element.forever.Worker.Worker"></a>[function <span class="apidocSignatureSpan">forever.</span>Worker (options)](#apidoc.element.forever.Worker.Worker)
- description and source-code
```javascript
Worker = function (options) {
  events.EventEmitter.call(this);
  options = options || {};

  this.monitor  = options.monitor;
  this.sockPath = options.sockPath || forever.config.get('sockPath');
  this.exitOnStop = options.exitOnStop === true;

  this._socket = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.Worker.super_"></a>[function <span class="apidocSignatureSpan">forever.Worker.</span>super_ ()](#apidoc.element.forever.Worker.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.Worker.prototype"></a>[module forever.Worker.prototype](#apidoc.module.forever.Worker.prototype)

#### <a name="apidoc.element.forever.Worker.prototype.start"></a>[function <span class="apidocSignatureSpan">forever.Worker.prototype.</span>start (callback)](#apidoc.element.forever.Worker.prototype.start)
- description and source-code
```javascript
start = function (callback) {
  var self = this,
      err;

  if (this._socket) {
    err = new Error("Can't start already started worker");
    if (callback) {
      return callback(err);
    }

    throw err;
  }

  //
  // Defines a simple 'nssocket' protocol for communication
  // with a parent process.
  //
  function workerProtocol(socket) {
    socket.on('error', function() {
      socket.destroy();
    });

    socket.data(['ping'], function () {
      socket.send(['pong']);
    });

    socket.data(['data'], function () {
      socket.send(['data'], self.monitor.data);
    });

    socket.data(['spawn'], function (data) {
      if (!data.script) {
        return socket.send(['spawn', 'error'], { error: new Error('No script given') });
      }

      if (self.monitor) {
        return socket.send(['spawn', 'error'], { error: new Error("Already running") });
      }

      var monitor = new (forever.Monitor)(data.script, data.args);
      monitor.start();

      monitor.on('start', function () {
        socket.send(['spawn', 'start'], monitor.data);
      });
    });

    socket.data(['stop'], function () {
      function onStop(err) {
        var args = [];
        if (err && err instanceof Error) {
          args.push(['stop', 'error'], { message: err.message, stack: err.stack });
          self.monitor.removeListener('stop', onStop);
        }
        else {
          args.push(['stop', 'ok']);
          self.monitor.removeListener('error', onStop);
        }

        socket.send.apply(socket, args);
        if (self.exitOnStop) {
          process.exit();
        }
      }

      self.monitor.once('stop', onStop);
      self.monitor.once('error', onStop);

      if (process.platform === 'win32') {
        //
        // On Windows, delete the 'symbolic' sock file. This
        // file is used for exploration during 'forever list'
        // as a mapping to the '\\.pipe\\*' "files" that can't
        // be enumerated because ... Windows.
        //
        fs.unlink(self._sockFile);
      }

      self.monitor.stop();
    });

    socket.data(['restart'], function () {
      self.monitor.once('restart', function () {
        socket.send(['restart', 'ok']);
      });

      self.monitor.restart();
    });
  }

  function findAndStart() {
    self._socket = nssocket.createServer(workerProtocol);
    self._socket.on('listening', function () {
      //
      // 'listening' listener doesn't take error as the first parameter
      //
      self.emit('start');
      if (callback) {
        callback(null, self._sockFile);
      }
    });

    self._socket.on('error', function (err) {
      if (err.code === 'EADDRINUSE') {
        return findAndStart();
      }
      else if (callback) {
        callback(err);
      }
    });

    //
    // Create a unique socket file based on the current microtime.
    //
    var sock = self._sockFile = path.join(self.sockPath, [
      'worker',
      new Date().getTime() + utile.randomString(3),
      'sock'
    ].join('.'));

    if (process.platform === 'win32') {
      //
      // Create 'symbolic' file on the system, so it can be later
      // found via "forever list" since the '\\.pipe\\*' "files" can't
      // be enumerated because ... Windows.
      //
      fs.openSync(sock, 'w');

      //
      // It needs the prefix, otherwise EACCESS error happens on Windows
      // (no .sock extension, only named pipes with .pipe prefixes)
      //
      sock = '\\\\.\\pipe\\' + sock;
    }

    self._socket.listen(sock);
  }

  //
  // Attempt to start the server the first time
  //
  findAndStart();
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.cli"></a>[module forever.cli](#apidoc.module.forever.cli)

#### <a name="apidoc.element.forever.cli.addColumn"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>addColumn (name)](#apidoc.element.forever.cli.addColumn)
- description and source-code
```javascript
addColumn = function (name) {
  if (checkColumn(name)) {
    var columns = forever.config.get('columns');

    if (~columns.indexOf(name)) {
      return forever.log.warn(name.magenta + ' already exists in forever');
    }

    forever.log.info('Adding column: ' + name.magenta);
    columns.push(name);

    forever.config.set('columns', columns);
    forever.config.saveSync();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.cleanLogs"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>cleanLogs ()](#apidoc.element.forever.cli.cleanLogs)
- description and source-code
```javascript
cleanLogs = function () {
  forever.log.silly('Tidying ' + forever.config.get('root'));
  forever.cleanUp(true).on('cleanUp', function () {
    forever.log.silly(forever.config.get('root') + ' tidied.');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.clear"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>clear (key)](#apidoc.element.forever.cli.clear)
- description and source-code
```javascript
clear = function (key) {
  if (reserved.indexOf(key) !== -1) {
    forever.log.warn('Cannot clear reserved config: ' + key.grey);
    forever.log.warn('Use 'forever set ' + key + '' instead');
    return;
  }

  updateConfig(function () {
    forever.log.info('Clearing forever config: ' + key.grey);
    forever.config.clear(key);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.config"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>config ()](#apidoc.element.forever.cli.config)
- description and source-code
```javascript
config = function () {
  var keys = Object.keys(forever.config.store),
      conf = cliff.inspect(forever.config.store);

  if (keys.length <= 2) {
    conf = conf.replace(/\{\s/, '{ \n')
               .replace(/\}/, '\n}')
               .replace('\\033[90m', '  \\033[90m')
               .replace(/, /ig, ',\n  ');
  }
  else {
    conf = conf.replace(/\n\s{4}/ig, '\n  ');
  }

  conf.split('\n').forEach(function (line) {
    forever.log.data(line);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.getOptions"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>getOptions (file)](#apidoc.element.forever.cli.getOptions)
- description and source-code
```javascript
getOptions = function (file) {
  var options = {},
      absFile = isAbsolute(file) ? file : path.resolve(process.cwd(), file),
      configKeys = [
        'pidFile', 'logFile', 'errFile', 'watch', 'minUptime', 'append',
        'silent', 'outFile', 'max', 'command', 'path', 'spinSleepTime',
        'sourceDir', 'workingDir', 'uid', 'watchDirectory', 'watchIgnore',
        'killTree', 'killSignal', 'id'
      ],
      specialKeys = ['script', 'args'],
      configs;

  //
  // Load JSON configuration values
  //
  if (path.extname(file) === '.json') {
    configs = shush(absFile);
    configs = !Array.isArray(configs) ? [configs] : configs;

    configs = configs.map(function (conf) {
      var mut = Object.keys(conf)
        .reduce(function (acc, key) {
          if (~configKeys.indexOf(key) || ~specialKeys.indexOf(key)) {
            acc[key] = conf[key];
          }

          return acc;
        }, {});

      if (!mut.script) {
        forever.log.error('"script" option required in JSON configuration files');
        console.log(prettyjson.render(mut));
        process.exit(1);
      }

      return mut;
    });
  } else {
    options.script = file;
  }

  //
  // First isolate options which should be passed to file
  //
  options.args = process.argv.splice(process.argv.indexOf(file) + 1);

  //
  // Now we have to force optimist to reparse command line options because
  // we've removed some before.
  //
  app.config.stores.argv.store = {};
  app.config.use('argv', argvOptions);

  configKeys.forEach(function (key) {
    options[key] = app.config.get(key);
  });

  options.watchIgnore         = options.watchIgnore || [];
  options.watchIgnorePatterns = Array.isArray(options.watchIgnore)
    ? options.watchIgnore
    : [options.watchIgnore];

  if (!options.minUptime) {
    forever.log.warn('--minUptime not set. Defaulting to: 1000ms');
    options.minUptime = 1000;
  }

  if (!options.spinSleepTime) {
    forever.log.warn([
      '--spinSleepTime not set. Your script',
      'will exit if it does not stay up for',
      'at least ' + options.minUptime + 'ms'
    ].join(' '));
  }

  function assignSpawnWith(options) {
    options.sourceDir  = options.sourceDir  || (file && file[0] !== '/' ? process.cwd() : '/');
    options.workingDir = options.workingDir || options.sourceDir;
    options.spawnWith  = { cwd: options.workingDir };
    return options;
  }

  if (configs && configs.length) {
    return configs.map(function (conf) {
      return assignSpawnWith(objectAssign(clone(options), conf));
    });
  }

  return [assignSpawnWith(options)];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.help"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>help ()](#apidoc.element.forever.cli.help)
- description and source-code
```javascript
help = function () {
  util.puts(help.join('\n'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.list"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>list ()](#apidoc.element.forever.cli.list)
- description and source-code
```javascript
list = function () {
  forever.list(true, function (err, processes) {
    if (processes) {
      forever.log.info('Forever processes running');
      processes.split('\n').forEach(function (line) {
        forever.log.data(line);
      });
    }
    else {
      forever.log.info('No forever processes running');
    }
  });
}
```
- example usage
```shell
...
  }
]
'''

### Using In Your Code
The forever module exposes some useful methods to use in your code. Each method returns an instance of an EventEmitter which emits
 when complete. See the [forever cli commands][2] for sample usage.

**Remark:** As of 'forever@0.6.0' processes will not automatically be available in 'forever.list()'. In order to get your processes
 into 'forever.list()' or 'forever list' you must instantiate the 'forever' socket server:

''' js
  forever.startServer(child);
'''

This method takes multiple 'forever.Monitor' instances which are defined in the 'forever-monitor' dependency.
...
```

#### <a name="apidoc.element.forever.cli.logFiles"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>logFiles (index)](#apidoc.element.forever.cli.logFiles)
- description and source-code
```javascript
logFiles = function (index) {
  if (typeof index !== 'undefined') {
    return;
  }

  var rows = [['   ', 'script', 'logfile']];
  index = 0;

  forever.list(false, function (err, processes) {
    if (!processes) {
      return forever.log.warn('No forever logfiles in ' + forever.config.get('root').magenta);
    }

    forever.log.info('Logs for running Forever processes');
    rows = rows.concat(processes.map(function (proc) {
      return ['[' + index++ + ']', proc.file.grey, proc.logFile.magenta];
    }));

    cliff.putRows('data', rows, ['white', 'grey', 'magenta']);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.logs"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>logs (index)](#apidoc.element.forever.cli.logs)
- description and source-code
```javascript
logs = function (index) {
  var options = {
      stream: app.argv.fifo,
      length: app.argv.number
  };

  forever.tail(index, options, function (err, log) {
    if (err) {
      return forever.log.error(err.message);
    }

    forever.log.data(log.file.magenta + ':' + log.pid + ' - ' + log.line);

  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.resetColumns"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>resetColumns ()](#apidoc.element.forever.cli.resetColumns)
- description and source-code
```javascript
resetColumns = function () {
  var columns = 'uid command script forever pid logfile uptime';

  forever.log.info('Setting columns: ' + columns.magenta);

  forever.config.set('columns', columns.split(' '));
  forever.config.saveSync();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.restart"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>restart (file)](#apidoc.element.forever.cli.restart)
- description and source-code
```javascript
restart = function (file) {
  var runner = forever.restart(file, true);
  runner.on('restart', function (processes) {
    if (processes) {
      forever.log.info('Forever restarted process(es):');
      processes.split('\n').forEach(function (line) {
        forever.log.data(line);
      });
    }
    else {
      forever.log.info('No forever processes running');
    }
  });

  runner.on('error', function (err) {
    forever.log.error('Error restarting process: ' + file.grey);
    forever.log.error(err.message);
    process.exit(1);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.restartAll"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>restartAll ()](#apidoc.element.forever.cli.restartAll)
- description and source-code
```javascript
restartAll = function () {
  var runner = forever.restartAll(true);
  runner.on('restartAll', function (processes) {
    if (processes) {
      forever.log.info('Forever restarted processes:');
      processes.split('\n').forEach(function (line) {
        forever.log.data(line);
      });
    }
    else {
      forever.log.info('No forever processes running');
    }
  });

  runner.on('error', function () {
    forever.log.info('No forever processes running');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.rmColumn"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>rmColumn (name)](#apidoc.element.forever.cli.rmColumn)
- description and source-code
```javascript
rmColumn = function (name) {
  if (checkColumn(name)) {
    var columns = forever.config.get('columns');

    if (!~columns.indexOf(name)) {
      return forever.log.warn(name.magenta + ' doesn\'t exist in forever');
    }

    forever.log.info('Removing column: ' + name.magenta);
    columns.splice(columns.indexOf(name), 1);

    forever.config.set('columns', columns);
    forever.config.saveSync();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.run"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>run ()](#apidoc.element.forever.cli.run)
- description and source-code
```javascript
run = function () {
  var file = app.argv._[0],
      options = getOptions(file);

  options.forEach(function (o) {
    tryStart(o.script, o, function () {
      var monitor = forever.start(o.script, o);
      monitor.on('start', function () {
        forever.startServer(monitor);
      });
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.set"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>set (key, value)](#apidoc.element.forever.cli.set)
- description and source-code
```javascript
set = function (key, value) {
  updateConfig(function () {
    forever.log.info('Setting forever config: ' + key.grey);
    forever.config.set(key, value);
  });
}
```
- example usage
```shell
...

#### forever.stop (index)
Stops the forever daemon script at the specified index. These indices are the same as those returned by forever.list(). This method
 returns an EventEmitter that raises the 'stop' event when complete.

#### forever.stopAll (format)
Stops all forever scripts currently running. This method returns an EventEmitter that raises the 'stopAll' event when complete.

The 'format' parameter is a boolean value indicating whether the returned values should be formatted according to the configured
 columns which can set with 'forever columns' or programmatically 'forever.config.set('columns')'.

#### forever.list (format, callback)
Returns a list of metadata objects about each process that is being run using forever. This method will return the list of metadata
 as such. Only processes which have invoked 'forever.startServer()' will be available from 'forever.list()'

The 'format' parameter is a boolean value indicating whether the returned values should be formatted according to the configured
 columns which can set with 'forever columns' or programmatically 'forever.config.set('columns')'.

#### forever.tail (target, options, callback)
...
```

#### <a name="apidoc.element.forever.cli.setColumns"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>setColumns (columns)](#apidoc.element.forever.cli.setColumns)
- description and source-code
```javascript
setColumns = function (columns) {
  forever.log.info('Setting columns: ' + columns.magenta);

  forever.config.set('columns', columns.split(' '));
  forever.config.saveSync();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.start"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>start ()](#apidoc.element.forever.cli.start)
- description and source-code
```javascript
start = function () {
  if (app.argv.version) {
    return console.log('v' + forever.version);
  }

  //
  // Check for --no-colors/--colors and --plain option
  //
  if ((typeof app.argv.colors !== 'undefined' && !app.argv.colors) || app.argv.plain) {
    colors.mode = 'none';
  }

  if (app.config.get('help')) {
    return util.puts(help.join('\n'));
  }

  app.init(function () {
    if (app.argv._.length && actions.indexOf(app.argv._[0]) === -1) {
      return cli.run();
    }

    app.start();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.startDaemon"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>startDaemon ()](#apidoc.element.forever.cli.startDaemon)
- description and source-code
```javascript
startDaemon = function () {
  var file = app.argv._[1],
      options = getOptions(file);

  options.forEach(function (o) {
    forever.log.info('Forever processing file: ' + o.script.grey);
    tryStart(o.script, o, function () {
      forever.startDaemon(o.script, o);
    });
  });

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.stop"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>stop (file)](#apidoc.element.forever.cli.stop)
- description and source-code
```javascript
stop = function (file) {
  var runner = forever.stop(file, true);

  runner.on('stop', function (process) {
    forever.log.info('Forever stopped process:' + '\n' + process);
  });

  runner.on('error', function (err) {
    forever.log.error('Forever cannot find process with id: ' + file);
    process.exit(1);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.stopall"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>stopall ()](#apidoc.element.forever.cli.stopall)
- description and source-code
```javascript
stopall = function () {
  var runner = forever.stopAll(true);
  runner.on('stopAll', function (processes) {
    if (processes) {
      forever.log.info('Forever stopped processes:');
      processes.split('\n').forEach(function (line) {
        forever.log.data(line);
      });
    }
    else {
      forever.log.info('No forever processes running');
    }
  });

  runner.on('error', function () {
    forever.log.info('No forever processes running');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.cli.stopbypid"></a>[function <span class="apidocSignatureSpan">forever.cli.</span>stopbypid (pid)](#apidoc.element.forever.cli.stopbypid)
- description and source-code
```javascript
stopbypid = function (pid) {
  forever.log.warn('Deprecated, try 'forever stop ' + pid + '' instead.');
  cli.stop(pid);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.log"></a>[module forever.log](#apidoc.module.forever.log)

#### <a name="apidoc.element.forever.log.data"></a>[function <span class="apidocSignatureSpan">forever.log.</span>data (msg)](#apidoc.element.forever.log.data)
- description and source-code
```javascript
data = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.debug"></a>[function <span class="apidocSignatureSpan">forever.log.</span>debug (msg)](#apidoc.element.forever.log.debug)
- description and source-code
```javascript
debug = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.error"></a>[function <span class="apidocSignatureSpan">forever.log.</span>error (msg)](#apidoc.element.forever.log.error)
- description and source-code
```javascript
error = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.help"></a>[function <span class="apidocSignatureSpan">forever.log.</span>help (msg)](#apidoc.element.forever.log.help)
- description and source-code
```javascript
help = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.info"></a>[function <span class="apidocSignatureSpan">forever.log.</span>info (msg)](#apidoc.element.forever.log.info)
- description and source-code
```javascript
info = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.input"></a>[function <span class="apidocSignatureSpan">forever.log.</span>input (msg)](#apidoc.element.forever.log.input)
- description and source-code
```javascript
input = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.prompt"></a>[function <span class="apidocSignatureSpan">forever.log.</span>prompt (msg)](#apidoc.element.forever.log.prompt)
- description and source-code
```javascript
prompt = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.silly"></a>[function <span class="apidocSignatureSpan">forever.log.</span>silly (msg)](#apidoc.element.forever.log.silly)
- description and source-code
```javascript
silly = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.verbose"></a>[function <span class="apidocSignatureSpan">forever.log.</span>verbose (msg)](#apidoc.element.forever.log.verbose)
- description and source-code
```javascript
verbose = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.log.warn"></a>[function <span class="apidocSignatureSpan">forever.log.</span>warn (msg)](#apidoc.element.forever.log.warn)
- description and source-code
```javascript
warn = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.forever.out"></a>[module forever.out](#apidoc.module.forever.out)

#### <a name="apidoc.element.forever.out.debug"></a>[function <span class="apidocSignatureSpan">forever.out.</span>debug (msg)](#apidoc.element.forever.out.debug)
- description and source-code
```javascript
debug = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.out.error"></a>[function <span class="apidocSignatureSpan">forever.out.</span>error (msg)](#apidoc.element.forever.out.error)
- description and source-code
```javascript
error = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.out.info"></a>[function <span class="apidocSignatureSpan">forever.out.</span>info (msg)](#apidoc.element.forever.out.info)
- description and source-code
```javascript
info = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.out.silly"></a>[function <span class="apidocSignatureSpan">forever.out.</span>silly (msg)](#apidoc.element.forever.out.silly)
- description and source-code
```javascript
silly = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.out.verbose"></a>[function <span class="apidocSignatureSpan">forever.out.</span>verbose (msg)](#apidoc.element.forever.out.verbose)
- description and source-code
```javascript
verbose = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.forever.out.warn"></a>[function <span class="apidocSignatureSpan">forever.out.</span>warn (msg)](#apidoc.element.forever.out.warn)
- description and source-code
```javascript
warn = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
