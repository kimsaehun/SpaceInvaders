# SpaceInvaders

[![Build Status](https://travis-ci.org/ivanperez-keera/SpaceInvaders.svg?branch=master)](https://travis-ci.org/ivanperez-keera/SpaceInvaders)
[![Version on Hackage](https://img.shields.io/hackage/v/SpaceInvaders.svg)](https://hackage.haskell.org/package/SpaceInvaders)

This is a Haskell Space Invaders game implemented using the Functional
Reactive Programming library Yampa.

The game has been created for educational purposes, but tries to feature a
substantial amount of the complexity often found in real arcade games. In
particular:

* Differentiated subsystems for physics/collisions, input,
  rendering/multimedia, logic, etc.

![SpaceInvaders on Debian](screenshots/debian.png?raw=true)

## Installation

The game will also be available on hackage. We personally recommend using sandboxes (either with cabal or with cabal-dev)*:

```
$ cabal update
$ cabal sandbox init                # skip if you are using cabal-dev
$ cabal unpack SpaceInvaders        # or git clone https://github.com/ivanperez-keera/SpaceInvaders.git
$ cd SpaceInvaders-*                    # Game resources are here
$ cabal install                     # ...or cabal-dev install
$ ./dist/build/spaceInvaders/spaceInvaders
```
 
## Documentation

To try and make things as clear as possible, the code includes a much haddock
documentation and comments as we could reasonably fit. You can compile those with:

```
$ cabal unpack SpaceInvaders     ## Or git clone this-repo
$ cd SpaceInvaders-*
$ cabal sandbox init
$ cabal install --only-dependencies
$ cabal configure && cabal haddock --executables --internal
```

## Related slides and projects

This game was used in a paper called The Yampa Arcade, by Henrik Nilsson ([details](http://www.cs.nott.ac.uk/~psznhn/papers.html#hw2003)). It is used to explain FRP to new audiences.
* [Slides from a 2003 talk](http://www.cs.nott.ac.uk/~psznhn/Talks/HW2003-YampaArcade.pdf)
* [More up to date slides but on FRP/Yampa more generally](   http://www.cs.nott.ac.uk/~psznhn/Talks/7digital-July2016-IntroductionToFRPAndYampaThroughGamesAndMusic.pdf) and as [handout](   http://www.cs.nott.ac.uk/~psznhn/Talks/7digital-July2016-IntroductionToFRPAndYampaThroughGamesAndMusic-4up.pdf). It makes some comparisons with Cycle.js and XStreams which might
    be useful to some readers.
* [More generally, this series of lectures of FRP including SpaceInvaders as an example.](http://www.cs.nott.ac.uk/~psznhn/ITU-FRP2010/ITU-FRP2010.html)
* Yampa (http://github.com/ivanperez-keera/Yampa), the Arrowized Functional
Reactive Programming implementation created by Antony Courtney and Henrik Nilsson.
* [Haskanoid](https://github.com/ivanperez-keera/haskanoid): a game that uses
  SDL multimedia, wiimote and kinect. It's cross platform and works in desktop,
  mobile, and [web](http://ivanperez-keera.github.io/haskanoid/haskanoid.jsexe/index.html)
  (compiled with [GHCJS](https://github.com/ghcjs/ghcjs)).
* Magic Cookies (https://github.com/keera-studios/magic-cookies), a commercial
  FRP game written in Haskell using Yampa that's available on
[iTunes](https://itunes.apple.com/us/app/magic-cookies/id1244709871) and
[Google
Play](https://play.google.com/store/apps/details?id=uk.co.keera.games.magiccookies&hl=en).

## Educators

If you find this game attractive and would like to use it to teach functional
programming or other subjects, we'd be very happy to know about it. We can
provide extra material that you can show to students (videos, screenshots,
etc.).

## Help and collaboration

You can collaborate at least in two ways:

* File an issue (https://github.com/ivanperez-keera/SpaceInvaders/issues).
* Write documentation (send a link and/or a pull request).

## Homework

We would like to call on Haskell programmers, game developers and anyone with
an interest in Functional Reactive Programming and/or Game Programming to
review the code, ask for clarification when the code is not clear enough, and
help us improve the game, and the state of FRP/Yampa programming as well.

## Author

* Henrik Nilsson

### Maintainer

* Ivan Perez

### Collaborators

* Christina Zeller