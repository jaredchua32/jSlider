JSlider constructor takes:
1. jQuery object of the <div class = "jSlider"></div>
2. urls of the images as an array
3. options object

* Fix css - location of leftArrow.png and rightArrow.png

==============================================
JSlider options

You may use the default settings I have provided, modify them for all JSlider instances, or give each JSlider instance its own settings. The default values for each property of the jSlider.options object are outlined in their respective section of this wiki page. The default settings can also be found at the bottom of jSlider.js.

You may easily override the settings for all instances of jSlider by modifying the properties of the $.jSlider.options object.

Example: change the frame background and top margin for all jSliders.
[code] $.jSlider.options.frameBG = 'rgba(123,123,123,1)'
		$.jSlider.options.marginTop = '75px'

Because the jSlider constructor accepts an options object, you may also override the default settings by passing in an object with all the properties that you wish to override.

Example: Override width, frame background, top margin, resize delay, disable navigation buttons, and disable the auto scroll feature.

[code] 
customOptions = {
	width: '720px',
	frameBG: '#FFFFFF',
	marginTop: '100px',
	resizeDelay: 100,
	navButtons: false,
	autoScroll: false
}

After creating the custom options object, simply pass it along with the jQuery object holding the container div and the array of image URLs to use for the slider. JSlider will take care of overriding the settings for you!
[code]
$.jSlider($container, arrayOfImages, customOptions);

The details of every setting in jSlider.options are outlined below.

width


width
default: width: 			'auto',
possible values:
description:

frameBG
default: frameBG: 		'#000000',
possible values:
description:

marginTop
default: marginTop: 		'50px',
possible values:
description:

resizeDelay
default: resizeDelay: 	50,
possible values:
description:

sideButtons
default: sideButtons: 	'auto',
possible values:
description:

leftBtn
default: leftBtn: 		undefined,
possible values:
description:

rightBtn
default: rightBtn: 		undefined,
possible values:
description:

navButtons
default: navButtons: 	true,
possible values:
description:

autoScroll
default: autoScroll: 	true,
possible values:
description:

scrollInterval
default: scrollInterval: 3000,
possible values:
description:

scrollDuration
default: scrollDuration: 600,
possible values:
description:

pauseDuration
default: easingpauseDuration: 	1000,
possible values:
description:

default: easing: 		'linear'
possible values:
description:

==============================================