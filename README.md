toast [![Code Climate](http://img.shields.io/codeclimate/github/tameraydin/toast.svg?style=flat)](https://codeclimate.com/github/tameraydin/toast/dist/toast.js) [![Build Status](http://img.shields.io/travis/tameraydin/toast/master.svg?style=flat)](https://travis-ci.org/tameraydin/toast)
=======

toast is a simple Angular provider for toast notifications.

**[Demo](http://tameraydin.github.io/ngToast)**

## Usage

1. Download:
  ```console
  bower install ngtoast
  ```
  or manually from [dist](https://github.com/tameraydin/toast/tree/master/dist).

2. Include toast source files and dependencies ([ngAnimate](http://docs.angularjs.org/api/ngAnimate), [ngSanitize](http://docs.angularjs.org/api/ngSanitize), [Bootstrap CSS](http://getbootstrap.com/)):
  ```html
  <link rel="stylesheet" href="bower/bootstrap/dist/css/bootstrap.min.css">
  <link rel="stylesheet" href="bower/ngtoast/dist/toast.min.css">
  
  <script src="bower/angular-animate/angular-animate.min.js"></script>
  <script src="bower/angular-sanitize/angular-sanitize.min.js"></script>
  <script src="bower/ngtoast/dist/toast.min.js"></script>
  ```
 *Note: only the [Alerts](http://getbootstrap.com/components/#alerts) component is used as style base, so you don't have to include complete CSS*

3. Include toast as a dependency in your application module:
  ```javascript
  var app = angular.module('myApp', ['toast']);
  ```

4. Place `ng-toast` element into your HTML:
  ```html
  <body>
    <ng-toast></ng-toast>
    ...
  </body>
  ```

5. Inject toast provider in your controller:
  ```javascript
  app.controller('myCtrl', function(toast) {
    toast.create('a toast message...');
  });
  ```

## Settings & API

Please find at the [project website](http://tameraydin.github.io/ngToast/#api).

## Development

* Install dependencies: `npm install`
* Play on **/src**
* Run `grunt`

## License

MIT [http://tameraydin.mit-license.org/](http://tameraydin.mit-license.org/)

## TODO
- Add unit & e2e tests
- Improve API documentation
