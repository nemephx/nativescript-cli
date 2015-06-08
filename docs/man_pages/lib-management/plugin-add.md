plugin add 
==========

Usage | Synopsis
------|-------
General | `$ tns plugin add <Plugin>`

<% if(isConsole) { %>Installs the specified plugin and any packages that it depends on.<% } %>  
<% if(isHtml) { %>Installs the specified plugin and its dependencies in the local `node_modules` folder, adds it to the `dependencies` section in `package.json`, and prepares the plugin for all installed platforms. For more information about working with plugins, see [NativeScript Plugins](https://github.com/NativeScript/nativescript-cli/PLUGINS.md).<% } %>

### Attributes

* `<Plugin>` is a valid NativeScript plugin, specified by any of the following.
    * A `<Name>` or `<Name>@<Version>` where `<Name>` is the name of a plugin that is published in the npm registry and `<Version>` is a valid version of this plugin.
    * A `<Local Path>` to the directory which contains the plugin, including its `package.json` file.
    * A `<Local Path>` to a `.tar.gz` archive containing a directory with the plugin and its `package.json` file.
    * A `<URL>` which resolves to a `.tar.gz` archive containing a directory with the plugin and its `package.json` file.
    * A `<git Remote URL>` which resolves to a `.tar.gz` archive containing a directory with the plugin and its `package.json` file.

<% if(isHtml) { %>
### Prerequisites

* Verify that the plugin that you want to add contains a valid `package.json` file. Valid `package.json` files contain a `nativescript` section.

### Related Commands

Command | Description
----------|----------
[library](library.html) | You must run the library command with a related command.
[library add](library-add.html) | Adds a native library to the current project.
[plugin](plugin.html) | Lists all installed plugins for your project or lets you manage the plugins for your project.
[plugin remove](plugin-remove.html) | Uninstalls the specified plugin and its dependencies.
<% } %>