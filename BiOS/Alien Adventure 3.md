# Project Overview
In this practice session, you will finish implementing a start menu and add a new “badge” gameplay element to the UI. There is also one method you will implement that corresponds to a request given by an alien.

The start menu and “badge” element will test your ability to work with Swift concepts like classes, inheritance, and Cocoa design patterns—specifically the target/action pattern. The single method will also reinforce these concepts. If you correctly implement the method as specified by the alien, then the robot hero will give a proper response and progress through that portion of the adventure. If the implementation is incorrect, then the robot hero will give an improper response and the adventure will end immediately.

For the start menu, you will be provided with a pre-existing view. After setting the start menu as the initial view for the app, you will add target/action pairs that correspond to events that take place in the UI—adjusting the level switch, adjusting the “Show Badges” switch, and pressing the “Start!” button.

To add the “badge” feature, you will be modifying two pre-existing classes. You will be responsible for creating custom initializers that load an image as a texture for a sprite. Also, you will create and use an enumeration type that supports the random playing of an animation.

# Completing this Project
You should have completed all the necessary steps for finishing this project in Alien Adventure 3 Prep. Before submitting, ensure your app does the following:

* The implementation of the `init(requestType: UDRequestType)` initializer for the `Badge` class correctly sets the `requestType` property and calls the superclass initializer providing a valid texture argument that uses the “BadgeMagenta” image.
* The implementation of the `init(requestType: UDRequestType)` initializer for the `SpecialBadge` class correctly overrides the `Badge` initializer and sets its texture to use the “BadgeTeal” image.
* A `BadgeAnimation` enum is defined in the `SpecialBadge` class such that it has a raw type of `Int` and has three cases: GrowAndShrink, Rotate, and Shake.
* The implementation of the `init(requestType: UDRequestType)` initializer for the `SpecialBadge` class randomly generates a `BadgeAnimation` and runs the associated animation.
* The implementation of the `checkBadges` method is correct and passes all acceptance tests.
* The `SettingsViewController` is presented as the initial view controller.
* The SettingsViewController has target/action pairs for the following events:
  * If the value changes for the `levelSegmentedControl`, then the `switchLevel` method is called.
  * If the value changes for the `showBadgesSwitch`, then the `showBadges` method is called.
  * If the `startGameButton` is touched, then the `startGame` method is called.
* The `SettingsViewController` correctly implements the following methods (actions):
  * The `switchLevel` method correctly adjusts the `Settings.Common.Level` variable.
  * The `showBadges` method correctly adjusts the `Settings.Common.ShowBadges` variable.
  * The `startGame` method starts the Alien Adventure game (instantiates and presents the `AlienAdventureViewController`).

# Submitting Your Project
Before submitting your project for evaluation, we recommend that you check that each of the following is true:

* Your app compiles & runs as expected
* You are proud of your app and its output
* You completed your project according to the instructions
* You checked your project against [the rubric](https://docs.google.com/document/d/1Hh1WIb-qUlsEKxDp3p--2AtndeUGhNoGC21R0nwSVpA/pub?embedded=true)

