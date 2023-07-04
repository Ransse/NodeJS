# npm cheat sheet

## npm help

*List npm usable commands*<br>
`npm help`

*Give different usage of npm install*<br>
`npm install -h`

*Goes through npm documentation to search for a certain text*<br>
`npm help-search update`

*Then use command command below to open documentation in browser*<br>
`npm help update`

## Package.json

*Initialise a new npm repo by creating package.json*<br>
`npm init`

*Same as commande above but skips all the questions during package.json creation*<br>
`npm init --yes`

## npm versioning

*Installing specific version of a package following the @*<br>
`npm install lodash@3.3.0 --save`

*Install a specific version taking the latest patch version*<br>
`npm install lodash@4.14 --save`

*Same as previous but taking latest major*<br>
`npm install lodash@4 --save`

## Installing from package.json

*Using ~ version before package version instead of ^ restricts the major and minor and take only the latest for patch version*<br>
> Ex: "lodash": "~4.14.1"

*You can install a specific package version by doing the following*<br>
> Ex: "lodash": "4.14.1"

*Retrieving the latest of major minor and patch*<br>
> Ex: "lodash": "*"

## Updating package version

*Updates lodash version based on the requirements set on the package.json*<br>
`npm update lodash --save`

*Updates all dev dependencies*<br>
`npm update --dev --save-dev`

*Updates all dependencies and dev dependencies*<br>
`npm update`

*For global dependencies*<br>
`npm update -g`

*Updates npm to the latest global*<br>
`npm install npm@latest -g`

## Npm prune

> **_NOTE:_**  `npm list --depth 0` can help you find extraneous packages installed in your node modules. An extraneous package is a direct package dependencies found in node modules but not present in package.json

*Removes extraneous packages*<br>
`npm prune`

## Npm shorthands

`npm init --yes` <=> `npm init -y`

`npm install lodash` <=> `npm i lodash`

`npm i lodash --save` <=> `npm i lodash -S`

`npm install moment --save-dev` <=> `npm i moment -D`
