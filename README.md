# Webcam manipulation with HTML5

This is an [AngularJS][] directive that can be added as a module to your own app.

Demos can be found at [http://jonashartmann.github.io/webcam-directive](http://jonashartmann.github.io/webcam-directive)

## Contribute

1. Fork and clone this repository
2. Install dependencies

		npm install
3. Build/test with grunt

		grunt [build|test]

The minified file can be found inside the dist folder.

## Download

#### The current version can be found inside the dist/ folder of this repo.
	Ex.: dist/<version_number>/webcam.min.js

## Installation

#### Using script tag
	<script type="text/javascript" src="webcam.min.js"></script>

## Usage

#### Add module "webcam" as dependency
    angular.module('myapp', ['webcam']);

#### Then just use the new element
    <webcam></webcam>

#### Callbacks
	<webcam on-stream="onStream(stream,video)"
	        on-access-denied="onError(err)"
	        on-streaming="onSuccess(video)">
	</webcam>
#### Custom placeholder to be shown while loading the webcam
    <webcam placeholder="'img/ajax-loader.gif'">

## Technologies used in this project

- [AngularJS][]
- [Yeoman](http://yeoman.io/)
- [getUserMedia](https://developer.mozilla.org/en-US/docs/WebRTC/navigator.getUserMedia)
- [canvas](https://developer.mozilla.org/en-US/docs/HTML/Canvas)
- [video](https://developer.mozilla.org/en-US/docs/HTML/Element/video)

The code is licensed under the MIT License. @see LICENSE file

[angularjs]:http://angularjs.org
