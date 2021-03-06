<p align="center">
  <img width="300" height="100" src="https://cdn.rawgit.com/ImXico/Cyberpunk/1458bf76/logo.svg">  
</p>
<p align="center">
  <a href="https://travis-ci.org/ImXico/Cyberpunk"><img src="https://travis-ci.org/ImXico/Cyberpunk.svg?branch=master"></a>
  <a href="http://libgdx.badlogicgames.com/"><img src="https://img.shields.io/badge/libgdx-1.9.8-red.svg"></a>
  <a href="https://kotlinlang.org/"><img src="https://img.shields.io/badge/kotlin-1.2.21-orange.svg"></a>
  <a href="https://jitpack.io/#ImXico/Cyberpunk"><img src="https://jitpack.io/v/ImXico/Cyberpunk.svg"></a>
  <a href="https://github.com/ImXico/HandyGDX/blob/master/LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
</p>

Cyberpunk is a collection of independent, modular, pure-Kotlin libraries to use on top of [libGDX](http://libgdx.badlogicgames.com/), tailored with Java interoperability in mind. By offering various utilities and boilerplates, it aims to speed up development and ease the making of prototypes, making it a great fit for game jams!

### Modules

Cyberpunk is all about small, independent modules. Because of the Gradle integration, you can import *just* the modules that you need. To properly serve that purpose, every single module is totally independent from all others.

Here are the **current** modules (each one has a *README.md* file):

- [audio](https://github.com/ImXico/Cyberpunk/tree/master/audio): Music/Sound asset management and various utilities.
- [camera](https://github.com/ImXico/Cyberpunk/tree/master/camera): Various camera styles on the go.
- [core](https://github.com/ImXico/Cyberpunk/tree/master/core): States, state management and transitions. Get up and running quickly!
- [image](https://github.com/ImXico/Cyberpunk/tree/master/image): Image asset management and various utilities.
- [physics](https://github.com/ImXico/Cyberpunk/tree/master/physics): Friendly and practical Box2D constructs.
- [text](https://github.com/ImXico/Cyberpunk/tree/master/text): Text positioning helpers.

### Usage

JitPack is used here, so, if you want to import *any* module, add this to your root `build.gradle` file:

```Groovy
allprojects {
  repositories {
    // ...
    maven { url 'https://jitpack.io' }
  }
}
```

Now, in order to import single modules, add to the `dependencies` as follows:

```Groovy
compile 'com.github.imXico.cyberpunk:$module:$version'
```

Replace `$module` with the name of the desired library (see above). Likewise, `$version` should be replaced with the desired version. Check out the released versions [here](https://github.com/ImXico/Cyberpunk/releases).

### What About libKTX?

Good question! Indeed, [libKTX](https://github.com/libktx/ktx) is an awesome project! If you're already a libKTX user and you're happy with it, you should definitely stick with it. Same thing would apply if you were to start a larger, *pure Kotlin* project. It provides an *incredible* range of utilities, and makes full use of Kotlin's awesome features!

That being said, if you're looking for a smoother Java interop or are carrying out a game jam, give Cyberpunk a try!

### Report Issues

Something not working quite as expected? Do you need a feature that has not been implemented yet? Feel free to report bugs, fix them, suggest enhancements, add functionality and point out any mistakes!

### License

This project is released under the MIT License.
