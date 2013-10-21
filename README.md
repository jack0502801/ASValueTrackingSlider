## ValueTrackingSlider
----
### What is it?
A UISlider Subclass that displays live values in a popUpView. It’s inspired by the implementation found [here](https://github.com/mneuwert/iOS-Custom-Controls), but this version is built using CALayers.
It’s designed for use with iOS7 (though with a few alterations, it should be simple enough to get working on iOS6 and below).

### Features

* Live updating of UISlider value
* Customizable text color and popUpView color
* Set your own NSNumberFormatter to control the displayed values
* Wholesome springy animation

### What do you need?
Just include these two files in your project:

* ASValueTrackingSlider.m and .h

### How to use it

It’s very simple. Just drag a UISlider into your Storyboard/nib and set it’s class to ASValueTrackingSlider.
The example below demonstrates how to customize the appearance and value displayed
```objective-c

self.slider.maximumValue = 255.0;

[self.slider setMaxFractionDigitsDisplayed:0];

[self.slider setPopUpViewColor:[UIColor colorWithHue:0.55 saturation:0.5 brightness:0.9 alpha:0.8]];

[self.slider setTextColor:[UIColor colorWithHue:0.55 saturation:1 brightness:0.4 alpha:1]];
```

