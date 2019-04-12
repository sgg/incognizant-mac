# incognizant-mac

## What is it? 

A dirt simple Chrome theme that changes the color of the frame in Incognito mode to a lovely orange.

## Why is it?

[Chrome 73](https://developers.google.com/web/updates/2019/03/nic73) introduced Dark Mode for Mac.
Regular windows look an awful lot (read: exactly) like Incognito windows when Dark Mode is enabled and 
unfortunately, Chrome 73 neglected to introduce a way to [_disable_ Dark Mode](https://bugs.chromium.org/p/chromium/issues/detail?id=948991).

1. I mostly like Dark Mode on OS X, but I don't like having my browser history further polluted with searches for [Rust Compiler Errors](https://doc.rust-lang.org/error-index.html).
2. Turns out creating a theme is waaaaaaay easier than maintaining a fork of Chromium so here we are.

## Who is it for?

Folks who use Dark Mode on OS X and want Incognito windows that are easily recognized.

## Caveats

* This totally violates Apple's [Visual Design Guidelines](https://developer.apple.com/design/human-interface-guidelines/macos/visual-design/color/) as it hardcodes the Dark Mode `systemOrangeColor`. As such it may look ugly on any version of OS X that isn't 10.14.3.
* The Native Theme in Chrome uses the system colors [dynamically](https://cs.chromium.org/chromium/src/ui/native_theme/native_theme_mac.mm) as it should. This theme doesn't.
* I have not tested this on any platforms (or even other computers) so caveat emptor.
