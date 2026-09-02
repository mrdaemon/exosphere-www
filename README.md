# exosphere-www

> THIS IS NOT A PLACE OF HONOR.
> NO HIGHLY ESTEEMED DEED IS COMMEMORATED HERE.
> WHAT IS HERE WAS DANGEROUS AND REPULSIVE TO US.
> THIS MESSAGE IS A WARNING ABOUT DANGER.

This repository unfortunately contains the source code for the
Exosphere mini site ([exosphere.tools](https://exosphere.tools)).

**As a disclaimer**: I am an old, grumpy nerd who remembers the old web and
absolutely hates modern frontend work, and only begrudgingly does it when
forced to, and muddles through by throwing stuff at the wall until it sticks.

This repository is probably deeply offensive to anyone who knows what they
are doing.

It is built with [Zola](https://www.getzola.org/), which ships a single static
binary with no other dependencies, unlike hugo which dips into Go modules very
very quickly, and end up introducing friction I did not need or want.

The entire goal was to keep it maintainable, simple, static and require as few
tools as possible to work on. SASS/SCSS was only allowed because Zola has a
built-in compiler and handles it on its own, and I refuse to involve node.

In short, I'm very sorry for whatever you encounter in here, and I won't be
offended if you run away screaming, because I also wanted to while writing the
horrifying hacks that make this work the way it does.

## Cheat Sheet

It's a Zola thing. You can run the Zola things.

```sh
zola serve
zola build
zola check
```

## The garbage layout

Because I wanted the data to be separate from the layout, most of the page is
configured through config.toml for glbal elements, and the prose is in markdown
files used as content blocks under `content/blocks/*.md`.

The blocks contain their own metadata if any, as front matter extras, and the
directory is set to `render = false` because they are not directly published or
actual pages. This generates some `Orphan page` warnings from Zola, which is
fine and harmless.

The templates under `templates/` are mostly just the layout, and explicitly load
the blocks where they belong. I felt almost comfortable making these. Almost.

The very small amount of Javascript is inlined at the bottom of templates,
where it is used, and I am once more, sorry in advance.

Everything else should be more or less self-explanatory. Maybe.

## The video demo

The demo gif was just ran through ffmpeg to produce a webm and mp4, and I
unfortunately already forgot how. Next time I make one, I'll probably generate
the files directly as part of the vhs recording process in the first place.

## Fonts, icons and licensing

The site is MIT licensed, much like Exosphere.

Source Code Pro is licensed under the SIL Open Font License 1.1, with the
license text in `static/fonts/source-code-pro/LICENSE.txt`. It is the same file
the documentation ships, and the CSS falls back to DejaVu Sans Mono, as is
tradition.

Platform icons come from [Simple Icons](https://simpleicons.org/) (CC0),
except `windows.svg`, which Simple Icons dropped somehow, and instead comes
from [Font Awesome Free](https://fontawesome.com/) (icons under CC BY 4.0).

The logos themselves remain trademarks of their respective projects and are
used here nominatively, to say what Exosphere runs on and manages.
