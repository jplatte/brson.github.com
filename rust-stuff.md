---
layout: basic
---

I've been [doing Rust](http://www.rust-lang.org/team.html) for [a
while
now](https://github.com/rust-lang/rust/commit/0633c7ae6e54edebde8421cef14267ad1ba1e30c). This
is where I remind myself of the good work I've done.

* Converted Rust from a statement language to an expression
  language.

* Introduced multithreading to the original (C++-based)
  green-threading runtime (along with [Eric
  Holk](http://github.com/eholk) and others), and [rewrote the runtime in
  Rust](https://mail.mozilla.org/pipermail/rust-dev/2013-August/005158.html). Most
  of this did not survive once green-threading was removed from Rust.

* Wrote the [segmented
  stack](https://mail.mozilla.org/pipermail/rust-dev/2013-November/006314.html)
  implementation of the green threading runtime.

* [Created the `Result`
  type](https://github.com/rust-lang/rust/commit/c1092fb6d88efe51e42df3aae2a321cc669e12a0),
  an alternative to Haskell's `Either` (which I *also* added to Rust,
  and later removed). Result was also [adopted by the Elm
  language](https://github.com/rust-lang/rust/commit/c1092fb6d88efe51e42df3aae2a321cc669e12a0).

* [Wrote the standard testing
  support](https://github.com/rust-lang/rust/commit/09982784c6ad1c78f9480c3c2c0c3a2b2bf7f969)
  along with
  [compiletest](https://github.com/rust-lang/rust/commit/2573fe7026eb696841acbba8f3d1c09e2224acf0),
  the first parallel Rust program.

* Wrote a lot of documentation.

* Created the original website that survived at least into 2015.

* Added an easter egg to the runtime that output [random Lovecraft
  quotes during fatal
  errors](https://github.com/brson/rust/blob/71a71ce4f948dd5ae792db4a88c9cc2fae94dfb0/src/libstd/rt/util.rs#L124).
  The worthiness of Lovecraft in a systems language was [hotly
  debated](https://news.ycombinator.com/item?id=8869572).

* Wrote much of the Rust build system, after
  [Graydon](http://github.com/graydon), which is a notoriously
  brain-searing abuse of make. It does though have an advanced
  [self-documenting](https://github.com/rust-lang/rust/blob/e4e93196e16030ebf7a20c473849534235d676f8/mk/main.mk#L592)
  help
  [system](https://github.com/rust-lang/rust/blob/e4e93196e16030ebf7a20c473849534235d676f8/Makefile.in#L11).
  That's my best idea there.

* I wrote the first version of rustdoc and created the original
  conventions for using Markdown in Rust doc comments. Rustdoc was
  later rewritten by [cmr](http://github.com/cmr/).

* I designed Rust's attributes.

* Maintained [This Week in Rust](http://this-week-in-rust.org), the
  Rust newsletter, along with [cmr](http://github.com/cmr/) and
  others. I believe the success of TWiR influenced the [proliferation
  of similar development
  newsletters](http://lwn.net/Articles/650527/).

* Created the [Friend of the
  Tree](https://github.com/rust-lang/rust-wiki-backup/blob/master/Doc-friends-of-the-tree.md)
  tradition (after Mozilla's own) for acknowleding community
  contributions.

* Created the Unix distribution tooling including
  [rustup.sh](http://github.com/rust-lang/rustup),
  [rust-installer](http://github.com/rust-lang/rust-installer) and
  [multirust](http://github.com/brson/multirust).

* Bootstrapped
  [Servo](https://github.com/servo/servo/graphs/contributors), the web
  browser written in Rust, along with
  [pcwalton](http://github.com/pcwalton) back when Rust barely worked.

* Established and supported Rust's community meetup tradition, with
  [Erick Tryzelaar](http://githtub.com/erickt) hosting the infamous
  [San Francisco Bay Area Rust
  Meetup](http://www.meetup.com/Rust-Bay-Area/) and supporting [many
  others](https://users.rust-lang.org/t/a-list-of-rust-1-0-launch-meetups/1171/16).

* Managed the release process [since the original 0.1
  release in January 2012](https://mail.mozilla.org/pipermail/rust-dev/2012-January/001256.html).