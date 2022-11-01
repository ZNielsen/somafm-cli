# somafm-cli <sub><sup>| Listen to SomaFM in your terminal via pure bash</sup></sub>
[![version](http://img.shields.io/badge/version-0.3.1-blue.svg)](https://github.com/rockymadden/somafm-cli/releases)
[![versioning](http://img.shields.io/badge/versioning-semver-blue.svg)](http://semver.org/)
[![branching](http://img.shields.io/badge/branching-github%20flow-blue.svg)](https://guides.github.com/introduction/flow/)
[![license](http://img.shields.io/badge/license-mit-blue.svg)](https://opensource.org/licenses/MIT)
[![gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/rockymadden/somafm-cli)
[![circleci](https://circleci.com/gh/rockymadden/somafm-cli.svg?style=shield)](https://circleci.com/gh/rockymadden/somafm-cli)

```console
$ somafm listen groovesalad
22:27:30 | Mindex - Jagga-jah
22:31:11 | Fresh Moods - Orfine
22:33:15 | Dr. Toast - Thunderclap
```

## Install
### Via Homebrew:
```console
$ brew tap rockymadden/rockymadden
$ brew install rockymadden/rockymadden/somafm-cli
```

### Via compiling from source:
```console
$ git clone git@github.com:rockymadden/somafm-cli.git
$ cd somafm-cli
$ make
$ make install
```
> __NOTE:__ Both `jq` and `mpv` are dependencies and without Homebrew you must ensure they are satisfied.

## Use
```console
$ somafm --help
Usage:
  somafm channels
  somafm listen <channel> [--quality=<low|high|highest>]

Options:
  quality    The listening quality (default: high)

Commands:
  channels|list|ls    List channels
  listen|play         Listen to channel
```

### Listen to Groove Salad:
```console
$ somafm listen groovesalad
22:27:30 | Mindex - Jagga-jah
```

You don't have to write the whole channel name, the first letters are enough.

```console
$ somafm listen groov
22:27:30 | Mindex - Jagga-jah
```

### Listen to Groove Salad at highest quality:
```console
$ somafm listen groovesalad --quality=highest
22:27:30 | Mindex - Jagga-jah
```

### List channels:
```console
$ somafm channels
groovesalad     1916 listeners  A nicely chilled plate of ambient/downtempo beats and grooves.
dronezone       883 listeners   Served best chilled, safe with most medications. Atmospheric textures with minimal beats.
spacestation    365 listeners   Tune in, turn on, space out. Spaced-out ambient and mid-tempo electronica.
deepspaceone    353 listeners   Deep ambient electronic, experimental and space music. For inner and outer space exploration.
indiepop        327 listeners   New and classic favorite indie pop tracks.
gsclassic       326 listeners   The classic (early 2000s) version of a nicely chilled plate of ambient/downtempo beats and grooves.
secretagent     300 listeners   The soundtrack for your stylish, mysterious, dangerous life. For Spies and PIs too!
lush            258 listeners   Sensuous and mellow female vocals, many with an electronic influence.
u80s            219 listeners   Early 80s UK Synthpop and a bit of New Wave.
seventies       181 listeners   Mellow album rock from the Seventies. Yacht not required.
defcon          151 listeners   Music for Hacking. The DEF CON Year-Round Channel.
synphaera       148 listeners   Featuring the music from an independent record label focused on modern electronic ambient and space music.
folkfwd         124 listeners   Indie Folk, Alt-folk and the occasional folk classics.
beatblender     123 listeners   A late night blend of deep-house and downtempo chill.
bootliquor      107 listeners   Americana Roots music for Cowhands, Cowpokes and Cowtippers
poptron         94 listeners    Electropop and indie dance rock with sparkle and pop.
suburbsofgoa    92 listeners    Desi-influenced Asian world beats and beyond.
thetrip         88 listeners    Progressive house / trance. Tip top tunes.
illstreet       80 listeners    Classic bachelor pad, playful exotica and vintage music of tomorrow.
sonicuniverse   79 listeners    Transcending the world of jazz with eclectic, avant-garde takes on tradition.
thistle         70 listeners    Exploring music from Celtic roots and branches
specials        57 listeners    For Halloween: Dark industrial/ambient music for tortured souls.
dubstep         55 listeners    Dubstep, Dub and Deep Bass. May damage speakers at high volume.
cliqhop         55 listeners    Blips'n'beeps backed mostly w/beats. Intelligent Dance Music.
christmas       55 listeners    Chilled holiday grooves and classic winter lounge tracks. (Kid and Parent safe!)
7soul           50 listeners    Vintage soul tracks from the original 45 RPM vinyl.
darkzone        49 listeners    The darker side of deep ambient. Music for staring into the Abyss.
reggae          49 listeners    Reggae, Ska, Rocksteady classic and deep tracks.
vaporwaves      43 listeners    All Vaporwave. All the time.
fluid           42 listeners    Drown in the electronic sound of instrumental hiphop, future soul and liquid trap.
brfm            38 listeners    From the Playa to the world, for the annual Burning Man festival.
missioncontrol  34 listeners    Celebrating NASA and Space Explorers everywhere.
sf1033          32 listeners    Ambient music mixed with the sounds of San Francisco public safety radio traffic.
digitalis       31 listeners    Digitally affected analog rock to calm the agitated heart.
covers          31 listeners    Just covers. Songs you know by artists you don't. We've got you covered.
metal           29 listeners    From black to doom, prog to sludge, thrash to post, stoner to crossover, punk to industrial.
xmasinfrisko    22 listeners    SomaFM's wacky and eclectic holiday mix. Not for the easily offended.
n5md            15 listeners    Emotional Experiments in Music: Ambient, modern composition, post-rock, & experimental electronic music
jollysoul       13 listeners    Where we cut right to the soul of the season.
xmasrocks       11 listeners    Have your self an indie/alternative holiday season!
live            11 listeners    Special Live Events and rebroadcasts of past live events
scanner         4 listeners     San Francisco Public Safety Scanner Feed
```

## License
```
The MIT License (MIT)

Copyright (c) 2018 Rocky Madden (https://rockymadden.com/)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
