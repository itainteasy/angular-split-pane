angular-split-pane
==================

An AngularJS Split Pane directive

The directive should work in IE8 and above as well as in Chrome, Safari and Firefox.

You can add angular-split-pane.js by to you project by installing with bower

    bower install angular-split-pane

Below is a basic example on how to use the directive. I'm using 

	<!DOCTYPE html>
	<html>
		<head>
			<meta charset="utf-8">
			<meta http-equiv="X-UA-Compatible" content="IE=edge">
			<title>Fixed left</title>
			<link rel="stylesheet" href="../bower_components/split-pane/split-pane.css" />
			<script src="../bower_components/jquery/dist/jquery.min.js"></script>
			<script src="../bower_components/angular/angular.js"></script>
			<script src="../bower_components/split-pane/split-pane.js"></script>
			<script src="../bower_components/angular-split-pane/angular-split-pane.js"></script>
			<style type="text/css">
				html, body {
					height: 100%;
					min-height: 100%;
					margin: 0;
					padding: 0;
				}
				/* The styling bolow is very simple. You can style things your own way. */
				body {
					box-sizing: border-box;
					background: #aaa;
					padding: 5px;
				}
				.split-pane-divider {
					background: #aaa;
				}
				.split-pane-component {
					background: #fff;
				}
			</style>
		</head>
		<body data-ng-app="example">
			<div data-split-pane>
				<div data-split-pane-component data-width="20em">left</div>
				<div data-split-pane-divider data-width="5px"></div>
				<div data-split-pane-component>right</div>
			</div>
			<script>
				angular.module('example', ['shagstrom.angular-split-pane']);
			</script>
		</body>
	</html>
