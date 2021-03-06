![Logo](admin/vis-material-advanced.png)
# ioBroker.vis-material-advanced

[![NPM version](http://img.shields.io/npm/v/iobroker.vis-material-advanced.svg)](https://www.npmjs.com/package/iobroker.vis-material-advanced)
[![Downloads](https://img.shields.io/npm/dm/iobroker.vis-material-advanced.svg)](https://www.npmjs.com/package/iobroker.vis-material-advanced)
![Number of Installations (latest)](http://iobroker.live/badges/vis-material-advanced-installed.svg)
![Number of Installations (stable)](http://iobroker.live/badges/vis-material-advanced-stable.svg)
[![Dependency Status](https://img.shields.io/david/EdgarM73/iobroker.vis-material-advanced.svg)](https://david-dm.org/EdgarM73/iobroker.vis-material-advanced)
[![Known Vulnerabilities](https://snyk.io/test/github/EdgarM73/ioBroker.vis-material-advanced/badge.svg)](https://snyk.io/test/github/EdgarM73/ioBroker.vis-material-advanced)

[![NPM](https://nodei.co/npm/iobroker.vis-material-advanced.png?downloads=true)](https://nodei.co/npm/iobroker.vis-material-advanced/)

## vis-material-advanced adapter for ioBroker

This Adapter provides standardized Widgets for vis in ioBroker. Lots of different predifined widgets

the basics of this adapter has been created by :
* (nisio) https://github.com/iobroker-community-adapters/ioBroker.vis-material
* (pix---) https://github.com/Pix---/ioBroker.vis-material

but rewritten in 90% 

Several bugfixes and lots of new widgets added 

## Attention, old widgets ( < 0.5.0 will be corrupted a little bit)
    you can repair them manually in vis or export them, edit them, and import them again.
    for manual : replace "opacity-color": "opac-<somecolor>" with "opacity-color": "<somecolor>". replace colorizeByTemp with colorizeByValue

    Example from sigi234 ( example.json ) and my example2.json are in the github for everybody who wants to test them

    Sorry for the inconveniance, but these changes were neccessary to keep code clean and understandable.

    this should not happen very often any more :)

## following widgets are present right now:

### current
 - Temperature
 - Humidity
 - Door
 - Window
 - Occupacy
 - Volume
 - Shutter
 - Light
 - Dimmer
 - Light-temperature
 - Boolean

### in progress
not yet final:
 - Garagedoor
 - Radiostation 


 lot of widgets still in plan

## Options
    following options are available in most of the widgets:
    
    - text-color
    - cord-icon ( does not yet make sense everywhere, e.g. dimmer )
    - opacity color ( the standard opacity color )
    - colorizeByValue ( depending on some values the opacity color can be changed e.g. if it is too hot make it red, to cold blue )
    - below,above, min, max ( the values for colorieByValue )
    - color-low/high,medium... ( the color to use if border is raised)
    - read-only ( some widgets can be set to read only mode for display only)


### Getting started

install the Adapter and start VIS in Edit mode.
On left side choose vis-material-adapter and than all widgets are shown in preview.

............. lots of docu missing ......................

**you can import the example.json file into vis**
thanks to @sigi234

## Changelog
<!--
    Placeholder
    ### __WORK IN PROGRESS__
-->


### 0.6.3 (2020-09-08)
* bugfix valve widget


### 0.6.1
* added two new widgets with complete new css-classes. rounded corner, two value. 

### 0.5.7
* bugfix number widget

### 0.5.6
* type in volume

### 0.5.5
* no icons anymore for text and number

## License
MIT License

Copyright (c) 2020 EdgarM73 <edgar.miller@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.