# requirejs-optional

Based on a [stackoverflow answer](http://stackoverflow.com/a/27422370/130480), loads a requirejs module optionally.

## Installation

    bower install requirejs-optional

## Usage

    require(['optional!jquery'], function(jquery){...});

`jquery` will be set to `undefined`.

## Remark

Due to the way requirejs and client application work, it *will* generate 404 calls when the module can't be found.