# EarlGrey Example

An example that shows several features of EarlGrey.

`EarlGreyExampleSwift` is an app written in Swift that provides a showcase test ground.

`EarlGreyExampleTests` and `EarlGreyExampleSwiftTests` are test targets that exercise
different functionalities provide by EarlGrey, written in Objective-C and Swift.

## Getting Started

### CocoaPods

Execute `gem install earlgrey` then `pod install --repo-update` from the directory where you have downloaded
the source of the example, then `open EarlGreyExample.xcworkspace` to open the example in xcode.
Ensure that your version of CocoaPods is upgraded to the latest 1.x version since this project uses the
[1.0.0 syntax](http://blog.cocoapods.org/CocoaPods-1.0/). You can get the latest CocoaPods release version by
running `gem install cocoapods`. The `--repo-update` flag is the same as `pod repo update`. This ensures the specs repository is aware of the latest version of EarlGrey. An old repo will result in downloading an old version of EarlGrey which may fail to compile with EarlGrey.swift.

Run the tests that you want to see in action.

### Carthage

From the directory containing the example source, run:

- `brew install carthage`
- `xcode-select --install`
- `gem install earlgrey`
- `earlgrey install --carthage --swift-version=3.0 --target=EarlGreyExampleSwiftTests`
- `carthage update EarlGrey --platform ios`
- `open EarlGreyExample.xcodeproj`

Xcode should now allow you to execute the EarlGreyExampleSwiftTests tests. If you get a compile error, try the following:

- Delete derived data
  - `rm -rf "$HOME/Library/Developer/Xcode/DerivedData"`
- Delete untracked and modified data
  - `git reset --hard; git clean -dfx`
