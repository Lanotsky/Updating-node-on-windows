# Updating-node-on-windows

If you want to update local NPM package on windows machine, either [Download](https://nodejs.org/en/download/) and run the latest MSI. The MSI will update your installed node and npm.

There is another solution, which will update npm package globally on local machine.

**Run PowerShell as Administrator**

`Set-ExecutionPolicy Unrestricted -Scope CurrentUser -Force
npm install -g npm-windows-upgrade
npm-windows-upgrade`

**Note**: Do not run npm i -g npm. Instead use npm-windows-upgrade to update npm going forward. Also if you run the NodeJS installer, it will replace the node version.

* Upgrades npm in-place, where node installed it.
* Easy updating, update to the latest by running npm-windows-upgrade -p -v latest.
* Does not modify the default path.
* Does not change the default global package location.
* Allows easy upgrades and downgrades.

Reference: [npm-windows-upgrade](https://github.com/felixrieseberg/npm-windows-upgrade)
