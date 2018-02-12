# Electrified Jailbreak Toolkit 
for iOS 11.0-11.1.2.
forked from coolstar's incredible basekit, Electra. you can find it at https://coolstar.org/electra/

---

This jailbreak is by the community, and was developed open source.

## Roadmap
See the [open issues](https://github.com/coolstar/electra/issues) for areas to be improved on.

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

### Planned:
- Dpkg/APT port (and maybe Cydia?) (coolstar)
- Structure filesystem more like a traditional jailbreak (coolstar)
- Fix user interface patterns (colordev)

## Contributing

* Download the repo, and run the code on your device.
* Make your patches
* PR!
* ???
* Profit :tada:

## I found a bug, how do I report it
[Open a new issue](https://github.com/coolstar/electra/issues/new), **after looking for similar issues already created.**

## Credits

This jailbreak was written by open source contributors. See [the contributors list](https://github.com/coolstar/electra/graphs/contributors) to find out who they are!

* jailbreakd and electra by ninjaprawn and coolstar
* cosmetic and futureproofing by colord3v
* kernel hang fixes by colord3v
* substitute changes for x and 8 by colord3v
* mobilesubstrate ports to substitute from saurik by colord3v

## License

Note: the async_awake exploit by Ian Beer is not licensed

However, for the additions by Electra, see LICENSE.md
