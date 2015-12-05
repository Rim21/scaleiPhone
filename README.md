#iOS scale a UI using Storyboard constraints

This is practice project #2 where I am demonstrating how I wish a UI to scale between iPhones from 3.5", 4", 4.7" and 5.5". The code that has been written is not a solution rather this code is the basis for discussion with like minded Devs. In other words the code is written by a beginner Dev in order to articulate a problem description and to seek help and ideas from others.

##Project setup

####There is no control code to this project - it is a storyboard UI prototype only project

###The UI consists of the following:

1.  a Display UIView - non working element
2.  a collection of buttons UIView - non working element
3.  a top Spacer UIView that is not visible on a 3.5" iPhone. This UIView has an App 'Title Text' as a Picture - non working element
4.  a middle Spacer UIView that is not visible on a 3.5" iPhone. This UIView has a 'separator' as a Picture - non working element
5.  a collection of buttons and a slider as a UIView - non working element
6.  a collection of 4 buttons roughly aligned horizontally. ***These are individual UI elements and are provided to enable the testing of horizontal stack views ***
7.  a bottom Spacer UIView that is not visible on a 3.5" iPhone. This UIView has an inverted 'separator' as a Picture - non working element

####It is anticipated that the vertical arrangements of the UI elements will enable the testing of vertical stack views

###Storyboard constraints:

1. all UIViews and buttons have constraints added. These were added through trial an error.
2.  the spacer Views are set to equal heights
3.  the buttons and UIViews constraints also include proportional width to superview
4.  the buttons also have a aspect ratio constraint
 
###Questions:

1. The approach taken for the spacer views throws an error in the Xcode console for the 3.5" screen size but still works. Is it better to use code to display/hide  these UI elements and if so what code is this? I make an assumption that I will need to look at UITraitcollection.... Swift code?
2. Stackviews are proving to be problematic because although I set the size of a button/UIView the stack view appears to strip away this setting and only uses the assets original size. This may be a function of the 'content hugging' property of UI stack views and the 'intrinsic' size of the asset. What is the best approach to overcoming the stack view problem?
