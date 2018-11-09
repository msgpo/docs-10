All SDK libraries available as pre-built packages on the GitHub [release page](https://github.com/mysteriumnetwork/node/releases).
It can be downloaded and installed manually with any preferred way.

But we also support several standard ways for installing SDK using dependency managers.

## iOS

It is possible to get iOS SDK library using [Carthage](https://github.com/Carthage/Carthage) dependency manager.

You can follow the [Carthage quick start guide] to get familiar how to use it or just use the following steps:

1. Carthage should be installed in the system.
2. `Cartfile` should be created in the same directory where `.xcodeproj` or `.xcworkspac` located.
3. `Cartfile` should contain the following line: `github "mysteriumnetwork/node" ~> 0.5.0`.
    - `mysteriumnetwork/node` - is a path to the GitHub [repository](https://github.com/mysteriumnetwork/node).
    - `0.5.0` - is a desired version of iOS SDK.

4. Execute command to get required library: `carthage update`.
5. A `Cartfile.resolved` file and a `Carthage` directory will appear in the same directory where your `.xcodeproj` or `.xcworkspace` is.
6. Drag the built `.framework` binaries from `Carthage/Build/<platform>` into your application’s Xcode project.

---

> *If you are going to use `dev` version of the SDK library `Cartfile` should contain version without postfix.*
> *For example, if you want to install `0.5-rc` version `Cartfile` should contain the following line: `github "mysteriumnetwork/node" ~> 0.5`.*

## Android

We are publishing an Android SDK library to the [Bintray](https://bintray.com/) repository. And as a result, it is available via [JCenter](https://bintray.com/bintray/jcenter) repository and can be easily imported into your project.

The Android SDK library available at [https://bintray.com/mysterium/Node/mobile-node](https://bintray.com/mysterium/Node/mobile-node)

All you need to do is just add the following line to your `build.gradle` file and resync it: `implementation 'mysterium.network:mobile-node:0.5-rc'`

---

> *It's also possible to install Android SDK library manually following official [guide](https://developer.android.com/studio/projects/android-library#AddDependency)*
