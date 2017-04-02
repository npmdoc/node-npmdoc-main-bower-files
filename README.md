# api documentation for  [main-bower-files (v2.13.1)](https://github.com/ck86/main-bower-files)  [![npm package](https://img.shields.io/npm/v/npmdoc-main-bower-files.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-main-bower-files) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-main-bower-files.svg)](https://travis-ci.org/npmdoc/node-npmdoc-main-bower-files)
#### Get main files from your installed bower packages.

[![NPM](https://nodei.co/npm/main-bower-files.png?downloads=true)](https://www.npmjs.com/package/main-bower-files)

[![apidoc](https://npmdoc.github.io/node-npmdoc-main-bower-files/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-main-bower-files_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-main-bower-files/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-main-bower-files/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Christopher Knötschke"
    },
    "bugs": {
        "url": "https://github.com/ck86/main-bower-files/issues"
    },
    "dependencies": {
        "chalk": "^1.0.0",
        "extend": "^2.0.1",
        "globby": "^2.0.0",
        "multimatch": "^2.0.0",
        "path-exists": "^1.0.0",
        "strip-json-comments": "^1.0.2",
        "vinyl-fs": "^2.4.3"
    },
    "description": "Get main files from your installed bower packages.",
    "devDependencies": {
        "grunt": "^0.4.5",
        "grunt-cli": "^0.1.13",
        "mocha": "^2.0.1",
        "should": "^7.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "7e1bc5c498352ccecd5df087f13d5f31bc057d3e",
        "tarball": "https://registry.npmjs.org/main-bower-files/-/main-bower-files-2.13.1.tgz"
    },
    "gitHead": "f2a1baa5de3227ba59ecc8df319cf7d6c58488ee",
    "homepage": "https://github.com/ck86/main-bower-files",
    "keywords": [
        "bower",
        "gulp",
        "gulpfriendly",
        "gruntplugin"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "cknoetschke",
            "email": "cknoetschke@gmail.com"
        },
        {
            "name": "trysound",
            "email": "trysound@yandex.ru"
        }
    ],
    "name": "main-bower-files",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ck86/main-bower-files.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "2.13.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module main-bower-files](#apidoc.module.main-bower-files)
1.  [function <span class="apidocSignatureSpan">main-bower-files.</span>package (opts, collection)](#apidoc.element.main-bower-files.package)
1.  [function <span class="apidocSignatureSpan">main-bower-files.</span>package_collection (opts)](#apidoc.element.main-bower-files.package_collection)
1.  object <span class="apidocSignatureSpan">main-bower-files.</span>package.prototype
1.  object <span class="apidocSignatureSpan">main-bower-files.</span>package_collection.prototype

#### [module main-bower-files.package](#apidoc.module.main-bower-files.package)
1.  [function <span class="apidocSignatureSpan">main-bower-files.</span>package (opts, collection)](#apidoc.element.main-bower-files.package.package)

#### [module main-bower-files.package.prototype](#apidoc.module.main-bower-files.package.prototype)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package.prototype.</span>addDependencies ()](#apidoc.element.main-bower-files.package.prototype.addDependencies)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package.prototype.</span>collectData ()](#apidoc.element.main-bower-files.package.prototype.collectData)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package.prototype.</span>getFiles (force)](#apidoc.element.main-bower-files.package.prototype.getFiles)

#### [module main-bower-files.package_collection](#apidoc.module.main-bower-files.package_collection)
1.  [function <span class="apidocSignatureSpan">main-bower-files.</span>package_collection (opts)](#apidoc.element.main-bower-files.package_collection.package_collection)

#### [module main-bower-files.package_collection.prototype](#apidoc.module.main-bower-files.package_collection.prototype)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>add (name, path, main)](#apidoc.element.main-bower-files.package_collection.prototype.add)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>addDependencies (dependencies, group, bowerJson)](#apidoc.element.main-bower-files.package_collection.prototype.addDependencies)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>checkGroupExists (group, bowerJson, error)](#apidoc.element.main-bower-files.package_collection.prototype.checkGroupExists)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>collectPackages ()](#apidoc.element.main-bower-files.package_collection.prototype.collectPackages)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>filterByGroup (deps, group, bowerJson)](#apidoc.element.main-bower-files.package_collection.prototype.filterByGroup)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>getFiles ()](#apidoc.element.main-bower-files.package_collection.prototype.getFiles)
1.  [function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>process ()](#apidoc.element.main-bower-files.package_collection.prototype.process)



# <a name="apidoc.module.main-bower-files"></a>[module main-bower-files](#apidoc.module.main-bower-files)

#### <a name="apidoc.element.main-bower-files.package"></a>[function <span class="apidocSignatureSpan">main-bower-files.</span>package (opts, collection)](#apidoc.element.main-bower-files.package)
- description and source-code
```javascript
function Package(opts, collection) {
    this.collection     = collection;
    this.name           = opts.name || null;
    this.path           = opts.path || null;
    this.main           = opts.main || null;
    this.dependencies   = opts.dependencies;
    this.ignore         = opts.ignore || false;
    this.debugging      = collection.debugging || false;

    if (this.ignore) {
        return;
    }

    this.collectData();
    this.addDependencies();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.main-bower-files.package_collection"></a>[function <span class="apidocSignatureSpan">main-bower-files.</span>package_collection (opts)](#apidoc.element.main-bower-files.package_collection)
- description and source-code
```javascript
function PackageCollection(opts) {
    this.opts               = opts;
    this.opts.main          = opts.main || null;
    this.opts.env           = opts.env || process.env.NODE_ENV;
    this.debugging          = opts.debugging || false;
    this.overrides          = opts.overrides || {};
    this._queue             = [];
    this._lastQueueLength   = 0;
    this._packages          = {};
    this._processed         = {};

    this.collectPackages();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.main-bower-files.package"></a>[module main-bower-files.package](#apidoc.module.main-bower-files.package)

#### <a name="apidoc.element.main-bower-files.package.package"></a>[function <span class="apidocSignatureSpan">main-bower-files.</span>package (opts, collection)](#apidoc.element.main-bower-files.package.package)
- description and source-code
```javascript
function Package(opts, collection) {
    this.collection     = collection;
    this.name           = opts.name || null;
    this.path           = opts.path || null;
    this.main           = opts.main || null;
    this.dependencies   = opts.dependencies;
    this.ignore         = opts.ignore || false;
    this.debugging      = collection.debugging || false;

    if (this.ignore) {
        return;
    }

    this.collectData();
    this.addDependencies();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.main-bower-files.package.prototype"></a>[module main-bower-files.package.prototype](#apidoc.module.main-bower-files.package.prototype)

#### <a name="apidoc.element.main-bower-files.package.prototype.addDependencies"></a>[function <span class="apidocSignatureSpan">main-bower-files.package.prototype.</span>addDependencies ()](#apidoc.element.main-bower-files.package.prototype.addDependencies)
- description and source-code
```javascript
addDependencies = function () {
    for (var name in this.dependencies) {
        this.collection.add(name, path.join(this.path, '..', name));
    }
}
```
- example usage
```shell
...
this.debugging      = collection.debugging || false;

if (this.ignore) {
    return;
}

this.collectData();
this.addDependencies();
};

Package.prototype = {
/**
 * Collects data from first found config file
 */
collectData: function() {
...
```

#### <a name="apidoc.element.main-bower-files.package.prototype.collectData"></a>[function <span class="apidocSignatureSpan">main-bower-files.package.prototype.</span>collectData ()](#apidoc.element.main-bower-files.package.prototype.collectData)
- description and source-code
```javascript
collectData = function () {
    var paths = [
            path.join(this.path, '.bower.json'),
            path.join(this.path, 'bower.json'),
            path.join(this.path, 'package.json'),
            path.join(this.path, 'component.json')
        ],
        data = paths.reduce(function(prev, curr) {
            if (prev && prev.main) {
                return prev;
            }

            if (!exists(curr)) {
                return prev;
            }

            try {
                return JSON.parse(readFile(curr, 'utf8'));
            } catch (e) {
                return null;
            }
        }, null);

    if (!data) {
        return;
    }

    if (!this.main && data.main) {
        this.main = data.main;

        if (this.debugging) {
            logger('Package', 'overriding main', this.name, data.main);
        }
    }

    if (!this.main && this.collection.opts.checkExistence) {
        throw new Error('Main property of package "' + this.name + '" is missing.');
    }

    if (this.dependencies === undefined && data.dependencies && data.dependencies) {
        this.dependencies = data.dependencies;

        if (this.debugging) {
            logger('Package', 'overriding dependencies', this.name, data.dependencies);
        }
    }
}
```
- example usage
```shell
...
this.ignore         = opts.ignore || false;
this.debugging      = collection.debugging || false;

if (this.ignore) {
    return;
}

this.collectData();
this.addDependencies();
};

Package.prototype = {
/**
 * Collects data from first found config file
 */
...
```

#### <a name="apidoc.element.main-bower-files.package.prototype.getFiles"></a>[function <span class="apidocSignatureSpan">main-bower-files.package.prototype.</span>getFiles (force)](#apidoc.element.main-bower-files.package.prototype.getFiles)
- description and source-code
```javascript
getFiles = function (force) {
    var main = this.main = this.main || this.collection.opts.main,
        files = [],
        name;

    if (main && typeof main === 'object' && !Array.isArray(main)) {
        main = main[this.collection.opts.env];
    }

    if (this.ignore || !main) {
        return files;
    }

    if (!Array.isArray(main)) {
        main = [main];
    }

    if (force !== true) {
        for (name in this.dependencies) {
            if (this.collection._processed[name] !== true) {
                return false;
            }
        }
    }

    main.forEach(function(pattern) {
        if (pattern[0] === '/') {
            throw new Error('absolute path in bower main is not supported');
        }

        var _files = globby(pattern, {
            cwd: this.path
        });

        if (!_files.length && this.collection.opts.checkExistence) {
            throw new Error('File on path "' + path.join(this.path, pattern) +
                '" does not exist.');
        }

        _files.forEach(function(file) {
            files.push(path.join(this.path, file));
        }, this);
    }, this);

    if (this.debugging) {
        files.forEach(function(file) {
            logger('Package', 'select file', this.name, file);
        }, this);
    }

    return files;
}
```
- example usage
```shell
...
        }

        this._lastQueueLength = queue.length;

        this._queue = [];

        queue.forEach(function(package) {
var packageSrcs = package.getFiles(force);

if (packageSrcs === false) {
    return this._queue.push(package);
}

srcs.push.apply(srcs, packageSrcs);
this._processed[package.name] = true;
...
```



# <a name="apidoc.module.main-bower-files.package_collection"></a>[module main-bower-files.package_collection](#apidoc.module.main-bower-files.package_collection)

#### <a name="apidoc.element.main-bower-files.package_collection.package_collection"></a>[function <span class="apidocSignatureSpan">main-bower-files.</span>package_collection (opts)](#apidoc.element.main-bower-files.package_collection.package_collection)
- description and source-code
```javascript
function PackageCollection(opts) {
    this.opts               = opts;
    this.opts.main          = opts.main || null;
    this.opts.env           = opts.env || process.env.NODE_ENV;
    this.debugging          = opts.debugging || false;
    this.overrides          = opts.overrides || {};
    this._queue             = [];
    this._lastQueueLength   = 0;
    this._packages          = {};
    this._processed         = {};

    this.collectPackages();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.main-bower-files.package_collection.prototype"></a>[module main-bower-files.package_collection.prototype](#apidoc.module.main-bower-files.package_collection.prototype)

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.add"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>add (name, path, main)](#apidoc.element.main-bower-files.package_collection.prototype.add)
- description and source-code
```javascript
add = function (name, path, main) {
    if (this._packages[name]) {
        return;
    }

    if (this.debugging) {
        logger('PackageCollection', 'add', name, path);
    }

    this._packages[name] = true;

    var opts = this.overrides[name] || {};
    opts.name = name;
    opts.path = path;
    if (path.indexOf(this.opts.paths.bowerDirectory) === -1) {
        opts.main = main || name;
    }
    opts.path = path;

    this._packages[name] = new Package(opts, this);
}
```
- example usage
```shell
...
},

/**
 * Adds package dependencies to the collection
 */
addDependencies: function() {
    for (var name in this.dependencies) {
        this.collection.add(name, path.join(this.path, '..', name));
    }
},

/**
 * Gets main files of the package
 *
 * @param  {Boolean}
...
```

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.addDependencies"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>addDependencies (dependencies, group, bowerJson)](#apidoc.element.main-bower-files.package_collection.prototype.addDependencies)
- description and source-code
```javascript
addDependencies = function (dependencies, group, bowerJson) {
    if (typeof dependencies !== "string") {
        var deps = (!!group) ? this.filterByGroup(dependencies, group, bowerJson) : dependencies;

        for (var name in deps) {
            this.add(name, path.join(this.opts.paths.bowerDirectory, path.sep, name));
        }
    } else {
        this.add(dependencies, path.join(path.dirname(this.opts.paths.bowerJson)));
    }
}
```
- example usage
```shell
...
this.debugging      = collection.debugging || false;

if (this.ignore) {
    return;
}

this.collectData();
this.addDependencies();
};

Package.prototype = {
/**
 * Collects data from first found config file
 */
collectData: function() {
...
```

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.checkGroupExists"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>checkGroupExists (group, bowerJson, error)](#apidoc.element.main-bower-files.package_collection.prototype.checkGroupExists)
- description and source-code
```javascript
checkGroupExists = function (group, bowerJson, error) {
    if(!group || !bowerJson.group) {
        return;
    }

    if (typeof group === "string") {
        var isExludingGroup = (group && bowerJson.group && group.charAt(0) === "!" && bowerJson.group[group.slice(1)].length > 0
);

        if(!bowerJson.group[group] && !isExludingGroup) {
            error(group);

            return;
        }

        return bowerJson.group[group];
    }

    if (typeof group === "object") {
        for (var i = 0; i < group.length; i++) {
            this.checkGroupExists(group[i], bowerJson, error);
        }
    }
}
```
- example usage
```shell
...
    dependencies = bowerJson.dependencies || {},
    main = bowerJson.main || {};

includeDev = includeDev === true ? 'inclusive' : includeDev;

this.overrides = extend(bowerJson.overrides || {}, this.overrides);

this.checkGroupExists(group, bowerJson, function (missingGroup) {
    throw new Error('group "' + missingGroup + '" does not exists in bower.json');
});

if (includeDev !== 'exclusive') {
    this.addDependencies(dependencies, group, bowerJson);
}
...
```

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.collectPackages"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>collectPackages ()](#apidoc.element.main-bower-files.package_collection.prototype.collectPackages)
- description and source-code
```javascript
collectPackages = function () {
    if (!exists(this.opts.paths.bowerJson)) {
        throw new Error('bower.json does not exist at: ' + this.opts.paths.bowerJson);
    }

    var name,
        group = this.opts.group || null,
        includeDev = this.opts.includeDev || false,
        includeSelf = this.opts.includeSelf || false,
        bowerJson = JSON.parse(stripJsonComments(readFile(this.opts.paths.bowerJson, 'utf8'))),
        devDependencies = bowerJson.devDependencies || {},
        dependencies = bowerJson.dependencies || {},
        main = bowerJson.main || {};

    includeDev = includeDev === true ? 'inclusive' : includeDev;

    this.overrides = extend(bowerJson.overrides || {}, this.overrides);

    this.checkGroupExists(group, bowerJson, function (missingGroup) {
        throw new Error('group "' + missingGroup + '" does not exists in bower.json');
    });

    if (includeDev !== 'exclusive') {
        this.addDependencies(dependencies, group, bowerJson);
    }

    if (includeDev !== false) {
        this.addDependencies(devDependencies, group, bowerJson);
    }

    if (includeSelf !== false) {
        this.add(bowerJson.name || 'self', path.dirname(this.opts.paths.bowerJson), main);
    }
}
```
- example usage
```shell
...
this.debugging          = opts.debugging || false;
this.overrides          = opts.overrides || {};
this._queue             = [];
this._lastQueueLength   = 0;
this._packages          = {};
this._processed         = {};

this.collectPackages();
};

PackageCollection.prototype = {
/**
 * Adds a package to the collection
 *
 * @param {String} name Name of the package
...
```

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.filterByGroup"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>filterByGroup (deps, group, bowerJson)](#apidoc.element.main-bower-files.package_collection.prototype.filterByGroup)
- description and source-code
```javascript
filterByGroup = function (deps, group, bowerJson) {
    var filtered = {};

    if (typeof group === "string") {
        var isExludingGroup = (group && bowerJson.group && group.charAt(0) === "!" && bowerJson.group[group.slice(1)].length > 0
);

        for (var dep in deps) {
            if (isExludingGroup && bowerJson.group[group.slice(1)].indexOf(dep) === -1) {
                filtered[dep] = deps[dep];
            }
            if (!isExludingGroup && bowerJson.group[group].indexOf(dep) >= 0) {
                filtered[dep] = deps[dep];
            }
        }

        return filtered;
    }

    if (typeof group === "object") {
        for (var i = 0; i < group.length; i++) {
            filtered = extend(filtered, this.filterByGroup(deps, group[i], bowerJson));
        }
    }

    return filtered;
}
```
- example usage
```shell
...

    /**
     * Adds all dependencies from list filtered by group
     *
     */
    addDependencies: function (dependencies, group, bowerJson) {
if (typeof dependencies !== "string") {
    var deps = (!!group) ? this.filterByGroup(dependencies, group, bowerJson) : dependencies;

    for (var name in deps) {
        this.add(name, path.join(this.opts.paths.bowerDirectory, path.sep, name));
    }
} else {
    this.add(dependencies, path.join(path.dirname(this.opts.paths.bowerJson)));
}
...
```

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.getFiles"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>getFiles ()](#apidoc.element.main-bower-files.package_collection.prototype.getFiles)
- description and source-code
```javascript
getFiles = function () {
    for (var name in this._packages) {
        this._queue.push(this._packages[name]);
    }

    return this.process();
}
```
- example usage
```shell
...
        }

        this._lastQueueLength = queue.length;

        this._queue = [];

        queue.forEach(function(package) {
var packageSrcs = package.getFiles(force);

if (packageSrcs === false) {
    return this._queue.push(package);
}

srcs.push.apply(srcs, packageSrcs);
this._processed[package.name] = true;
...
```

#### <a name="apidoc.element.main-bower-files.package_collection.prototype.process"></a>[function <span class="apidocSignatureSpan">main-bower-files.package_collection.prototype.</span>process ()](#apidoc.element.main-bower-files.package_collection.prototype.process)
- description and source-code
```javascript
process = function () {
    var queue = this._queue,
        srcs = [],
        force = false;

    if (this._lastQueueLength === queue.length) {
        force = true;
    }

    this._lastQueueLength = queue.length;

    this._queue = [];

    queue.forEach(function(package) {
        var packageSrcs = package.getFiles(force);

        if (packageSrcs === false) {
            return this._queue.push(package);
        }

        srcs.push.apply(srcs, packageSrcs);
        this._processed[package.name] = true;
    }, this);

    if (this._queue.length) {
        srcs.push.apply(srcs, this.process());
    }

    return srcs;
}
```
- example usage
```shell
...
 * @return {Array}
 */
getFiles: function() {
    for (var name in this._packages) {
        this._queue.push(this._packages[name]);
    }

    return this.process();
},

/**
 * processes the queue and returns the srcs of all packages
 *
 * @private
 * @return {Array}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
