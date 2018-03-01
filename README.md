# Electrified Jailbreak Toolkit 
for iOS 11.0-11.1.2.
(yes it was originally Electra)

---

This jailbreak is fueled by the community and maintained by colord3v.

## Roadmap
See the [open issues](https://github.com/colord3v/electra/issues) for areas to be improved on.

If you have a crash, PLEASE REPORT IT! otherwise I'll never know

### Currently implemented:
- setuid(0) - no panic
- KCALL - call kernel functions given an address and up to six arguments
- mount / as rw
- amfi bypass? well, run unsigned code (temporary until i figure out a master process which gives everyone everything with the right entitlements etc.)
- amfi**d** fixing up
- jailbreakd that keeps tfp0 task port open and runs a local server listening for commands
- Basic dylib injection into running process
- Working setuid (after calling jailbreakd to fix it up)
- Dpkg/APT/GPG port to iOS 11
- Cydia port (for now)
- Filesystem restructured temporarily, can be reverted with unjailbreak.sh
- MobileTerminal access
- Dropbear removed, OpenSSH added

### Planned:
- ????
- User interface tweaks

## I'm a developer, how do I update my tweaks and apps to support Electrified and MobileSubstitute?
Refer to our [getting started](docs/getting-started.md) guide for developers.

## Contributing

* Download the repo, and run the code on your device.
* Make your patches
* PR!
* ???
* Profit :tada:

## I found a bug, how do I report it
[Open a new issue](https://github.com/colord3v/electra/issues/new), **after looking for similar issues already created.**

## Credits

This jailbreak is based off of the developer only jailbreak toolkit [Electra](https://github.com/coolstar/electra) by coolstar and [async_wake](https://github.com/benjibobs/async_wake) by Ian Beer. 

* jailbreakd and electra by ninjaprawn and coolstar
* cosmetic and futureproofing by colord3v
* kernel hang fixes by colord3v
* substitute changes for x and 8 by colord3v
* mobilesubstrate ports to substitute from saurik by colord3v

## License

Note: the async_awake exploit by Ian Beer is not licensed

However, for the additions by Electra, see LICENSE.md

## Installation to End-User Devices

I've tried to make installation from GitHub as easy as possible.

If you don't know how to compile an IPA from this repo, here's all you need to do.

* Download a .zip of this repo from GitHub
* Make sure Windows Explorer (or Nautilius, Finder, whatever your cup of tea) is showing file extensions so the file is called "electrified-master.zip" instead of just "electrified-master"
* Rename the .zip to a .ipa
* Your new file should be *electrified-master.ipa* 
* Sideload to your iOS device running iOS 11.0-11.1.2 via Cydia Impactor or Xcode
