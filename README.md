WordCram lets you generate [word
clouds](http://images.google.com/images?q=word+cloud) in Processing.
It does the heavy lifting -- text analysis, collision detection -- for
you, so you can focus on making your word clouds as beautiful, as
revealing, or as silly as you like.

http://wordcram.googlecode.com/svn/javadoc/wordcram.png ![Word Cloud
by
WordCram](https://github.com/danbernier/WordCram/raw/master/wordcram.png)

Watch WordCram in action, on OpenProcessing: [popular baby
names](http://openprocessing.org/visuals/?visualID=12562), and [the
U.S. Constitution](http://openprocessing.org/visuals/?visualID=12413).

## Make a Word Cloud

```java
import wordcram.*;

// Set up the Processing sketch
size(1000, 600);
colorMode(HSB);
background(230);

// Make a wordcram from a random wikipedia page.
new WordCram(this)
  .fromWebPage("http://en.wikipedia.org/wiki/Special:Random")
  .withColors(color(30), color(110),
              color(random(255), 240, 200))
  .sizedByWeight(5, 120)
  .withFont("Copse")
  .drawAll();
```

You can control where words appear, what angle they're at, their font,
their color, and how they're sized.

## Install

[Installing](http://code.google.com/p/wordcram/wiki/Installing)
WordCram is simple, like any standard Processing library.

## How do I use this thing? Show me examples!

More of these are coming to the wiki, soon! But if you add WordCram to
Processing, you can see a bunch of examples under File > Examples >
Contributed Libraries > WordCram.

## Problems?

If you're running into problems, see the
[FAQ](http://code.google.com/p/wordcram/wiki/FAQ), or read the
[javadocs](http://wordcram.googlecode.com/svn/javadoc/index.html).

If a question has you stumped, and the
[FAQ](https://github.com/danbernier/WordCram/wiki/FAQ) is no help,
send me a note. My email account is 'wordcram', and I use gmail.

## Want a better WordCram?

WordCram is open-source under the Apache 2 license. That means you can
help make it better! I try to keep the source clean so it's easy to
find your way around. There's a [laundry list of things to
do](http://code.google.com/p/wordcram/wiki/ToDos), and it's easy to
[build WordCram from
source](http://code.google.com/p/wordcram/wiki/BuildingWordCram).