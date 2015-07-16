Caisson is a Cocoa framework that can be dropped into a MacOSX application to provide unobtrusive[1](1.md) crash and feedback reporting to a project in ActiveReload's [Lighthouse](http://www.lighthouseapp.com/) issue tracking service.

![http://myskitch.com/mattmower/lighthousetestapp_has_detected_that_it_crashed-20070709-174430.jpg](http://myskitch.com/mattmower/lighthousetestapp_has_detected_that_it_crashed-20070709-174430.jpg)

To implement crash reporting add the framework to your project in XCode, instante an LKReporter object, and set two framework specific properties in Info.plist. To add feedback tracking wire up a menu item to the appropriate action in the LKReporter object. It can't be much simpler.

Caisson has been modelled on the excellent [Sparkle auto-update framework](http://sparkle.andymatuschak.org/) by Andy Matuschack and would not have been considerably more difficult to implement if Andy had not generously made the source available. Thank you Andy.

[1](1.md) Caisson does not require any additional system components to be installed and does not use input managers or other hacks which might affect other applications.