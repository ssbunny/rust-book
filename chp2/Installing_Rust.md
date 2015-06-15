# Installing Rust

The first step to using Rust is to install it! There are a number of ways to install Rust, but the easiest is to use the `rustup` script. If you're on Linux or a Mac, all you need to do is this (note that you don't need to type in the `$`s, they just indicate the start of each command):


```sh
$ curl -sf -L https://static.rust-lang.org/rustup.sh | sh
```


If you're concerned about the potential insecurity of using `curl | sh`, please keep reading and see our disclaimer below. And feel free to use a two-step version of the installation and examine our installation script:


```sh
$ curl -f -L https://static.rust-lang.org/rustup.sh -O
$ sh rustup.sh
```

If you're on Windows, please download either the [32-bit installer](https://static.rust-lang.org/dist/rust-1.0.0-beta-i686-pc-windows-gnu.msi) or the [64-bit installer](https://static.rust-lang.org/dist/rust-1.0.0-beta-x86_64-pc-windows-gnu.msi) and run it.

## Uninstalling

If you decide you don't want Rust anymore, we'll be a bit sad, but that's okay. Not every programming language is great for everyone. Just run the uninstall script:


```sh
$ sudo /usr/local/lib/rustlib/uninstall.sh
```

If you used the Windows installer, just re-run the `.msi` and it will give you an uninstall option.

Some people, and somewhat rightfully so, get very upset when we tell you to `curl | sh`. Basically, when you do this, you are trusting that the good people who maintain Rust aren't going to hack your computer and do bad things. That's a good instinct! If you're one of those people, please check out the documentation on building Rust from Source, or the official binary downloads.


Oh, we should also mention the officially supported platforms:

* Windows (7, 8, Server 2008 R2)
* Linux (2.6.18 or later, various distributions), x86 and x86-64
* OSX 10.7 (Lion) or greater, x86 and x86-64

We extensively test Rust on these platforms, and a few others, too, like Android. But these are the ones most likely to work, as they have the most testing.

Finally, a comment about Windows. Rust considers Windows to be a first-class platform upon release, but if we're honest, the Windows experience isn't as integrated as the Linux/OS X experience is. We're working on it! If anything does not work, it is a bug. Please let us know if that happens. Each and every commit is tested against Windows just like any other platform.

If you've got Rust installed, you can open up a shell, and type this:


```sh
$ rustc --version
```

You should see the version number, commit hash, commit date and build date:

```sh
rustc 1.0.0-beta (9854143cb 2015-04-02) (built 2015-04-02)
```

If you did, Rust has been installed successfully! Congrats!

This installer also installs a copy of the documentation locally, so you can read it offline. On UNIX systems, `/usr/local/share/doc/rust` is the location. On Windows, it's in a `share/doc` directory, inside wherever you installed Rust to.

If not, there are a number of places where you can get help. The easiest is the #rust IRC channel on irc.mozilla.org, which you can access through Mibbit. Click that link, and you'll be chatting with other Rustaceans (a silly nickname we call ourselves), and we can help you out. Other great resources include the user’s forum, and Stack Overflow.





