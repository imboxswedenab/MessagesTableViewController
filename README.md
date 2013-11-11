# JSMessagesViewController [![Build Status](https://secure.travis-ci.org/jessesquires/MessagesTableViewController.png)](http://travis-ci.org/jessesquires/MessagesTableViewController)

A messages UI for iPhone and iPad.

![Messages Screenshot 1][img1] &nbsp;&nbsp;&nbsp; ![Messages Screenshot 2][img2]

`JSMessagesViewController` is a `UITableViewController` subclass that is very similar to the iOS Messages app. **Note, this is only a messaging UI, not a messaging app.**

**See more [screenshots](https://github.com/jessesquires/MessagesTableViewController/tree/master/Screenshots) in the `Screenshots/` directory.**

## Update!

####Version 3.0.0 just released with a brand new API! iOS 7 support + documentation coming soon!

## Features 

* Highly customizable
* Arbitrary message sizes
* Copy & paste messages
* Support for group messages
* Data detectors (recognizes phone numbers, links, dates, etc)
* Timestamps
* Avatars
* Subtitles
* Lots of bubble styles, or use your own!
* Swipe down to hide keyboard
* Dynamically resizes input text view as you type
* Smooth animations
* Automatically enables/disables send button (if text view is empty or not)
* Send/Receive sound effects
* Storyboards support (if that's how you roll)
* Universal

## Requirements

* iOS 6.0+ 
* ARC

## Installation

### From [CocoaPods](http://www.cocoapods.org)

    pod 'JSMessagesViewController'

### From source

* Drag the `JSMessagesViewController/` folder to your project.
* Add the `AudioToolbox.framework` to your project, if you want to use the sound effects

## Getting Started

1. Subclass `JSMessagesViewController`

2. In `- (void)viewDidLoad`
	* Set your view controller as the `delegate` and `datasource`
	* Set your view controller `title`

3. Implement the `JSMessagesViewDelegate` protocol

4. Implement the `JSMessagesViewDataSource` protocol

5. Implement `- (NSInteger)tableView:(UITableView *)tableView numberOfRowsInSection:(NSInteger)section` from the [`UITableViewDataSource` protocol](https://developer.apple.com/library/ios/documentation/uikit/reference/UITableViewDataSource_Protocol/Reference/Reference.html).

666. Present your subclassed ViewController programatically or via StoryBoards. Your subclass should be the `rootViewController` of a `UINavigationController`.

7. Read the documentation (Yes, there's documentation! Seriously!)

8. See the included demo project: `JSMessagesDemo.xcodeproj`

## Documentation

Documentation is [available here](http://cocoadocs.org/docsets/JSMessagesViewController) via [CocoaDocs](http://cocoadocs.org). Thanks [@CocoaDocs](https://twitter.com/CocoaDocs)!

## Customization

*Stuff here coming soon!*

## How To Contribute

*Stuff here coming soon!*

## Credits

Created by [Jesse Squires](https://twitter.com/jesse_squires), a [programming-motherfucker](http://programming-motherfucker.com).

Originally inspired by [@soffes](http://github.com/soffes)/[SSMessagingViewController][ss].

Many thanks to [le contributors](https://github.com/jessesquires/MessagesTableViewController/graphs/contributors) of this project.

Square message bubbles designed by [@michaelschultz](http://www.twitter.com/michaelschultz).

## About

I initialily developed this control to use in [Hemoglobe](http://www.hemoglobe.com) for private messages between users.

As it turns out, messaging is a popular thing that iOS devs want to do — I know, this is *shocking*. Thus, I am supporting this project in my free time and have added features way beyond what [Hemoglobe](http://www.hemoglobe.com) ever needed.

Check me out my work at [Hexed Bits](http://www.hexedbits.com).

## Apps Using This Control

[Hemoglobe](http://bit.ly/hemoglobeapp)

[Oxwall Messenger](https://github.com/tochman/OxwallMessenger)

[FourChat](https://itunes.apple.com/us/app/fourchat/id650833730?mt=8)

[Libraries for developers](https://itunes.apple.com/us/app/libraries-for-developers/id653427112?mt=8)

*[Contact me](mailto:jesse.squires.developer@gmail.com) to have your app listed here.*

## Related Projects

[SSMessagingViewController][ss]

[AcaniChat](https://github.com/acani/AcaniChat)

[UIBubbleTableView](https://github.com/AlexBarinov/UIBubbleTableView)

## [MIT License](http://opensource.org/licenses/MIT)

You are free to use this as you please. **No attribution necessary, but much appreciated.**

Copyright &copy; 2013 Jesse Squires

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[ss]:https://github.com/soffes/ssmessagesviewcontroller

[img1]:https://raw.github.com/jessesquires/MessagesTableViewController/master/Screenshots/iphone5-screenshot0.png
[img2]:https://raw.github.com/jessesquires/MessagesTableViewController/master/Screenshots/iphone5-screenshot2.png
