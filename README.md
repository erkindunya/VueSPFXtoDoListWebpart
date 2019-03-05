# Todo Client Web Part built with Vue.js and Vue's single-file components

## Summary

Sample Todo web part demonstrating how you can utilize [Vue](https://vuejs.org/v2) (a progressive framework for building user interfaces) with SharePoint Framework using handy [single-file components](https://vuejs.org/v2/guide/single-file-components.html) approach. 

## Used SharePoint Framework Version
![drop](https://img.shields.io/badge/drop-ga-green.svg)

## Applies to

* [SharePoint Framework Developer Preview](http://dev.office.com/sharepoint/docs/spfx/sharepoint-framework-overview)
* [Office 365 developer tenant](http://dev.office.com/sharepoint/docs/spfx/set-up-your-developer-tenant)

## Solution

Solution|Author(s)
--------|---------
vuejs-todo-single-file-component|Sergei Sergeev ([@sergeev_srg](https://twitter.com/sergeev_srg)), Dimcho Tsanov ([Singens](http://singens.com))

## Version history

Version|Date|Comments
-------|----|--------
0.0.1|January 27, 2017|Initial version.
0.0.2|March 30, 2017|Updated to GA
0.0.3|June 14, 2017|Fix webpack 2 issues
0.0.4|October 7, 2017|Updated packages to latest versions, misc fixing
0.0.5|November 15, 2017|Added data provider that demonstrates the CRUD operations
0.0.6|December 11, 2018|Updated sample to SPFx 1.4 and Vue 2.5.x

## Disclaimer
**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**

---

## Minimal Path to Awesome

- Clone this repo
- In the command line run:
  - `npm i`
  - `gulp serve`


## vue-j-senver

This is where you include your WebPart documentation.

### Building the code

```bash
git clone the repo
npm i
npm i -g gulp
gulp
```
```
Create new empty directory and run:
yo @microsoft/sharepoint

First of all, install vue from npm:
npm install vue --save
Then install webpack-merge module as developer dependency from npm:
npm install webpack-merge --save-dev
```

```
** Only run the GULP SERVE ON NODE COMMAND SHELL **

```
GIT error and fixes

	1. Does not work in Node 10 (Assertion `args[1]->IsString()' 
	
	From <https://github.com/karma-runner/karma/issues/3051> 
	src\node_contextify.cc:628: Assertion `args[1]->IsString()' failed.
	Use "npm install natives"
	
	From <https://github.com/karma-runner/karma/issues/3051> 
	2. Vue Packages version mismatch after upgrading to 2.4.3
	
	Try to delete the node_modules folder and the lock and reinstall.
	
	rm -rf ./node_modules yarn.lock && yarn install
	
	Or 
yarn.lock && yarn install

```
**ref:**
 https://spblog.net/post/2017/01/31/SharePoint-Framework-building-hello-world-web-part-with-Vuejs#continue

```
Note: You may face issue on saving but close the webbench and rerun
```
**gulp serve **
** it should work**
```

This package produces the following:

* lib/* - intermediate-stage commonjs build artifacts
* dist/* - the bundled script, along with other resources
* deploy/* - all resources which should be uploaded to a CDN.

### Build options

gulp clean - TODO
gulp test - TODO
gulp serve - TODO
gulp bundle - TODO
gulp package-solution - TODO


## Features

Demonstrates\uses below features:

 - integration between third party frontend framework Vue.js and SharePoint Framework
 - build pipeline customization
 - custom build pipeline tasks
 - modern component-based architecture
 - separation of concerns between markup, styling and code
 - single-file components architecture for Vue.js
 - custom webpack loaders

 <img src="https://telemetry.sharepointpnp.com/sp-dev-fx-webparts/samples/vuejs-todo-single-file-component" />
