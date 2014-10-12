Description
===========

Installs and configures redo - a system for building target files from source files, see the [[upstream],http://homepage.ntlworld.com/jonathan.deboynepollard/Softwares/redo.html] website for more details.

Requirements
============

A c++ compiler such as G++ or clang++.

Platform
--------

* Ubuntu 12.04, 14.04

**Notes**: This cookbook has been tested on the listed platforms. It
  may work on other platforms with or without modification.

Cookbooks
---------

* build-essential

Attributes
==========

default
-------

The following attributes are used, and we are attemping to replicate a slashpackage install with exported symlinks into /usr/local, by default.

* `node['redo']['source_url']` - The URL where the redo package can be retrieved from
* `node['redo']['prefix']` - The location given to the export script to install binaries/manpages to.

Recipes
=======

default
-------

Includes the `build-essential::default` recipe.  Builds and installs redo in the slashpackage manner if it is not already present.

License and Author
==================

Author:: Kevin Berry <kevin@opensourcealchemist.com>

Copyright 2014, Kevin Berry

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
