# requirejs-optional

Based on a [stackoverflow answer](http://stackoverflow.com/a/27422370/130480) by user [LordOfThePigs](http://stackoverflow.com/users/80779/lordofthepigs), loads a requirejs module optionally.

## Installation

    bower install requirejs-optional

Then, you can add `optional` in the paths configuration of requirejs this way:

    paths: {
        'optional': 'path_to_bower_components/requirejs-optional/dist/optional'
    } 

## Usage

    require(['optional!jquery'], function(jquery){...});

`jquery` will be set to `undefined`.

## Remark

Due to the way requirejs and client application work, it *will* generate 404 calls when the module can't be found.