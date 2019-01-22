# Pandoc CSS for Hakyll

`Drop-in` CSS for code highlighting in [Hakyll](https://jaspervdj.be/hakyll/).
Extracted from `pandoc` (`skylighting`) thanks to
[this blog](http://fixpt.de/blog/2017-12-03-hakyll-highlighting-themes.html).

#### Long story

[Hakyll](https://jaspervdj.be/hakyll/) is a Haskell library for generating static sites which uses
[Pandoc](https://pandoc.org/) for code syntax highlighting. But `Hakyll` by default does not include any CSS
for highlighting your code. So even if pandoc adds CSS classes to the generated HTML, you won't be able to see any
highlighting. This is probably because Hakyll wants users to have control of how to style their blog.

But the problem is CSS for pandoc is [not easily available](https://www.google.com/search?q=pandoc+css) that is
when I stumbled upon [this blogpost](http://fixpt.de/blog/2017-12-03-hakyll-highlighting-themes.html).

Interstingly pandoc uses [Skylighting](https://github.com/jgm/skylighting) internally which comes bundled with a
bunch of themes. But those themes are not readily available as CSS files in the repo - they are
[generated from code](https://github.com/jgm/skylighting/blob/master/skylighting-core/src/Skylighting/Styles.hs).
That blogpost explained how to generate CSS from `Skylighting`. So I went ahead and generated them for all
available themes! :tada:

## Usage

Look at the screenshots below, pick up [css file](/css) for the one you like and drop into your css.

## Screenshots

Here's how they look:

1. **breezeDark**

    ![breezeDark theme screenshot](/screenshots/breezeDark.png)

1. **espresso**

    ![espresso theme screenshot](/screenshots/espresso.png)

1. **haddock**

    ![haddock theme screenshot](/screenshots/haddock.png)

1. **kate**

    ![kate theme screenshot](/screenshots/kate.png)

1. **monochrome**

    ![monochrome theme screenshot](/screenshots/monochrome.png)

1. **pygments**

    ![pygments theme screenshot](/screenshots/pygments.png)

1. **tango**

    ![tango theme screenshot](/screenshots/tango.png)

1. **zenburn**

    ![zenburn theme screenshot](/screenshots/zenburn.png)
