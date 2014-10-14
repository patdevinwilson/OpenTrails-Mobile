OpenTrails Mobile
=============

Added a development branch.

OpenTrails Mobile is a [PhoneGap/Cordova](https://github.com/phonegap) app designed to offer trail visitors a useful map of the trail system in their region, offline, across devices. 

OpenTrails Mobile is a reference implementation of [OpenTrails (the Open Trail System Specification)](http://codeforamerica.org/specifications/trails), a data format developed by Code for America partners in Northeast Ohio, with guidance from the National Recreation and Parks Association, [GreenInfo Network](https://github.com/greeninfo), and [ESRI R&D in Portland](https://github.com/esripdx), among many others. OpenTrails Mobile can be configured to consume OpenTrails from the API of your choice.

At present, OpenTrails Mobile has only been thoroughly tested on iOS devices. 

![to-the-trails-screens](https://cloud.githubusercontent.com/assets/2983464/3578741/31691f04-0bb0-11e4-93aa-f72f09a88a50.png)

## Installation

**Note: the following requires that nodejs is installed, follow the [node installation instructions](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager) for your system if needed.**


Install the project dependencies with:

```
npm install
```

Once you have Cordova installed, clone the GitHub repo. **In the following command, change `YOUR_PROJECTS_DIRECTORY` to the directory you want the project to be downloaded into**:

```
git clone https://github.com/codeforamerica/trails-mobile ~/YOUR_PROJECTS_DIRECTORY/trails-mobile
```

Now navigate to the directory with:

```
cd ~/YOUR_PROJECTS_DIRECTORY/trails-mobile
```

To build and launch the application from the source code and view it in the iOS emulator, use:

```
./node_modules/.bin/cordova build ios
./node_modules/.bin/cordova emulate ios
```

If you'd prefer to view it in a web browser use:

```
./node_modules/.bin/cordova serve ios
```

Then to view the application visit `localhost:8000/ios/www/` in your web browser.

**If you'd prefer not to have to type out the node modules path each time, you'll need to add the node modules directory `./node_modules/.bin` to your PATH environment variable.**

## Development

If you work on the project and update the less file in `www/less/application.less` run `grunt less` to compile the CSS changes, or `grunt watch` to continuously compile the CSS changes while you work.

You can check JavaScript code quality by running `grunt jshint`.

##Contribution

  * Fork the project.
  * Make your feature addition or bug fix and commit the changes.
  * Send a pull request. Bonus points for topic branches.
