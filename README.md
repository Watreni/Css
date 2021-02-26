@import url(https://fonts.googleapis.com/css?family=Open+Sans:400,700);
body {
	background-color: rgb(237, 237, 237);
}
h1 {
	font-family: 'Open Sans', sans-serif;
	font-size: 13pt;
	font-weight: 600;
	text-transform: uppercase;
	color: rgb(255, 255, 255);
	cursor: default;
}
h4 {
	font-family: 'Open Sans', sans-serif;
	font-size: 8pt;
	font-weight: 400;
	cursor: default;
}
h2 {
	font-family: 'Open Sans', sans-serif;
	font-size: 13pt;
	font-weight: 300;
	color: rgb(255, 255, 255);
	cursor: default;
}
.player {
	height: 190px;
	width: 430px;
	background-color: rgb(30, 33, 37);
	position: absolute;
	-webkit-touch-callout: none;
	-webkit-user-select: none;
	-moz-user-select: none;
	-ms-user-select: none;
	user-select: none;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	-webkit-transform: translate(-50%, -50%);
	border-radius: 5px;
	border-top-left-radius: 100px;
	border-bottom-left-radius: 100px;
}
.player ul {
	list-style: none;
}
.player ul li {
	display: inline-block;
}
#arm{
	width: 90px;
	height: 90px;
	position: absolute;
	z-index: 1;
	top: 15px;
	left: 110px;
	transform-origin: 77.5% 18.5%;
	transform: rotate(-45deg);
	background-image: url(https://i.imgur.com/Bzzqadh.png);
	background-size: cover;
}
.artwork {
	position: absolute;
	top: 0;
	left: 0;
	height: 190px;
	width: 190px;
	background: url(https://i.imgur.com/3idGgyU.png), url(https://i.imgur.com/Fu2Oezw.png) center no-repeat;
	background-size: 190px, 75px !important;
}
.artwork img {
  position: absolute;
  height: 72px;
  width: 72px;
  border-radius: 50px;
  top: 59px;
  left: 59px;
}
.info h1 {
	margin: 0 0 -10px;
	margin-left: 180px;
	width: 182px;
	overflow: hidden;
	white-space: nowrap;
	text-overflow: ellipsis;
}
.info h4 {
	line-height: 20px;
	color: rgb(99, 99, 103);
	margin-left: 180px;
	width: 182px;
	overflow: hidden;
	white-space: nowrap;
	text-overflow: ellipsis;
}
.info h2 {
	margin-left: 180px;
	width: 182px;
	overflow: hidden;
	white-space: nowrap;
	text-overflow: ellipsis;
}
.button-items {
	margin-left: 180px;
}
#slider {
	width: 182px;
	height: 4px;
	background: rgb(21, 21, 24);
	border-radius: 2px;
	overflow: hidden;
}
#slider #elapsed {
	width: 0px;
	height: 4px;
	background: rgb(239, 109, 188);
	border-radius: 2px;
}
#slider #buffered {
	width: 0px;
	height: 4px;
	background: rgba(239, 109, 188, 0.3);
	border-radius: 2px;
	margin-top: -4px;
}
#timer {
	color: rgb(99, 99, 103);
	line-height: 0;
	font-size: 9pt;
	float: right;
	font-family: Arial, Sans-Serif;
}
.controls {
	margin-top: 25px;
}
.controls svg:nth-child(2) {
	margin-left: 5px;
	margin-right: 5px;
}
#play {
	padding: 0 3px;
	width: 30px;
	height: 30px;
	x: 0px;
	y: 0px;
	enable-background: new 0 0 25 25;
}
#play g {
	stroke: rgb(254, 254, 254);
	stroke-width: 1;
	stroke-miterlimit: 10;
}
#play g path {
	fill: rgb(254, 254, 254);
}

#play:hover {
	cursor: pointer;
}
#play:hover g {
	stroke: rgb(239, 109, 188);
	cursor: pointer;
}
#play:hover g path {
	fill: rgb(239, 109, 188);
	cursor: pointer;
}
.step-backward {
	width: 18px;
	height: 18px;
	x: 0px;
	y: 0px;
	enable-background: new 0 0 25 25;
	margin-bottom: 5px;
}
.step-backward g polygon, .step-foreward g polygon {
	fill: rgb(254, 254, 254);
}
.step-foreward {
	width: 18px;
	height: 18px;
	x: 0px;
	y: 0px;
	enable-background: new 0 0 25 25;
	margin-bottom: 5px;
}
#pause {
	x: 0px;
	y: 0px;
	enable-background: new 0 0 25 25;
	width: 30px;
	height: 30px;
	position: absolute;
	margin-left: -41px;
	cursor: pointer;
}
#pause rect {
	fill: rgb(255, 255, 255);
}

#pause:hover rect {
	fill: rgb(239, 109, 188);
}
.expend {
	padding: 0.5px;
	cursor: pointer;
}
.expend svg:hover g polygon {
	fill: rgb(239, 109, 188);
	cursor: pointer;
}
.slider {
	width: 80px;
	position: absolute;
	display: inline-block;
	margin: 4px 0 0 10px;
}
.slider .volume{
	width: 69px;
	height: 4px;
	background: rgba(239, 109, 188, 0.3);
	border-top-left-radius: 2px;
	border-bottom-left-radius: 2px;
	margin-top: 10px;
	position: inherit;
	pointer-events: none;
}
@-moz-document url-prefix() { //fix firefox being 1px off
	.slider .volume{
		margin-top: 11px;
	}
}
input[type="range"] {
	-webkit-appearance: none;
	-webkit-tap-highlight-color: rgba(255, 255, 255, 0);
	width: 100%;
	height: 4px;
	margin: 0;
	border: none;
	border-radius: 14px;
	padding: 0px 1px;
	background: rgb(21, 21, 24);
	outline: none;	
}
input[type="range"]::-moz-range-track {
	border: inherit;
	background: rgba(0, 0, 0, 0);
}
input[type="range"]::-ms-track {
	border: inherit;
	color: rgba(0, 0, 0, 0);
	background: rgba(0, 0, 0, 0);
}
input[type="range"]::-ms-fill-lower, input[type="range"]::-ms-fill-upper {
	background: rgba(0, 0, 0, 0);
}
input[type="range"]::-ms-tooltip {
	display: none;
}
input[type="range"]::-webkit-slider-thumb {
	-webkit-appearance: none;
	width: 12px;
	height: 12px;
	border: none;
	border-radius: 6px;
	background-color: rgb(255, 255, 255);
}
input[type="range"]::-moz-range-thumb {
	width: 12px;
	height: 12px;
	border: none;
	border-radius: 6px;
	background-color: rgb(255, 255, 255);
}
input[type="range"]::-ms-thumb {
	width: 12px;
	height: 12px;
	border-radius: 6px;
	border: 0;
	background-color: rgb(255, 255, 255);
}
input[type="range"]::-webkit-slider-thumb:hover, input[type="range"]::-webkit-slider-thumb:focus, input[type="range"]::-webkit-slider-thumb:active {
	background-color: rgb(239, 109, 188);
}
input[type="range"]::-moz-range-thumb:hover, input[type="range"]::-moz-range-thumb:focus, input[type="range"]::-moz-range-thumb:active {
	background-color: rgb(239, 109, 188);
}
input[type="range"]::-ms-thumb:hover, input[type="range"]::-ms-thumb:focus, input[type="range"]::-ms-thumb:active {
	background-color: rgb(239, 109, 188);
}
