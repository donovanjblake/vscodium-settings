# vscodium-settings

A repository containing my prefered VSCodium extensions and settings.

## Preferred Extensions

I primarily use rust, so I've included rust-analyzer and event-better-toml.

I find the Bearded Themes to be pleasant without being bland.

I have also included prettier-vscode because I prefer how it formats markdown documents.

## Syntax Highlighting

### Why

Broadly, I've chosen colors that help me read code quickly and understand what is happening. This
led to a goal of having more important items stand out, and ensuring items have high contrast with
one another.

This second point is one that I feel most themes fail on, in the interest of being more
aesthetically pleasing. It looks nice, but when keywords, variables, and types are slightly
different shades of blue, the code is a lot harder to quickly glance at and see the structure.
I also tried to avoid making the color set bright and loud and incoherent. It should still be
gentle on the eyes. You will find neither white nor black are used, nor is bold used.

### TL;DR

- Keywords are orange
- Variables are blue
- Functions are green
- Strings are yellow
- Types are purple
- Literals are brown
- Comments are gray

### Color Details

- Keywords are orange
  - But not traffic cone orange.
  - They are the anchors of the code, and orange gives that strong stable vibe.
- Variables are light blue
  - Variables are everywhere, but they are important.
  - They can't be too high contrast, or they will take over the screen.
  - They can't be too low contrast, or they will be hard to see.
  - They don't do things on their own, so they aren't an "actiony" color.
  - Members are like variables, so they are a slightly darker blue and italicized.
- Functions are light green
  - Functions are everywhere, but they are important.
  - They are higher contrast than variables because they actually do something.
  - They get an "actiony" color. Green means go.
  - Methods are like functions, so they are italicized.
- Strings are yellow
  - Idk man strings have always been yellow to me.
  - That's about all I've got for you.
- Types are purple
  - Hopefully your code doesn't have too many types, and most of them can be inferred by the
    compiler or interpreter.
  - They are rare, and generally don't bear the weight of what is happening.
  - They are a lower contrast color.
  - Type parameters are italicized.
- Literals are brown
  - Like strings, I dont have much of reason for this. Numbers are just brown to me.
  - Decimal, hexadecimal, float, don't care. Straight to brown.
  - Enumerators are like numbers in a lot of languages, so they are italicized.
- Comments are grey
  - I used to give comments a super high contrast, but I found them distracting me from the actual
    code too often when perusing a document. This led me to give them a much lower contrast color.
  - Comments are also italicized.
- In addition
  - Macros are magenta. Macros are evil, so they get the evil color.
  - Namespaces are gray because they generally aren't that important for reading what's happening.
  - Traits are the same purple as types. This may change in the future.
  - Escape codes in strings are basically numbers, so they get the same brown as numbers.

### Other Notes

- Why not use more shades? E.g. in some themes interfaces are a slighlty different shade from types.
  > I've stuck with a small-ish subset of colors, and avoided letting shades mean things because it
  > muddles the view. Keeping the selection of colors and shades minimal ensures that each item has
  > high contrast with its neighbors, instead of becoming an accidental gradient. Shades are also
  > used by code editors, e.g. desaturating/darkening code that's not in use, and I didn't want to
  > step on that.
- The defaults in the bearded theme have constants underlined. Why did you remove that?
  > I've avoided using bold and underline because I feel they are even more high contrast than high
  > contrast, and will be too distracting when trying to read code. Also, IMO good code is flooded
  > with constants to prevent accidental mutation, and that's way too many underlines. Code editors
  > also use squiggle underlines to signify things, and I didn't want to step on that.
- Whats with the brown enumerators?
  > Enumerators are basically just named numbers (in some languages). In rust, even though
  > enumerators are much more than names for literal integers, I've decided to stick with the
  > italic brown both because I was already used to it and because I think it makes a the pattern
  > of `Enum::Member(InnerType)` very legible with the purple-brown-purple contrast, instead of
  > just being a bunch of purple.
