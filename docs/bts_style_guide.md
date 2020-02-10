---
layout: ratyear
date: 2017-12-05
update: 2020-02-10
title: Style guide
description: Like every project worth its salt, The Photographers Field Guide to Beijing needed its own style guide. I took my sticky notes and wrote this up for my editor. Maybe you'll find it useful, too.
cta: <a href="mailto:hello@zachmccabe.com?Subject=Hi%20via%20{{ page.title }}">hello@zachmccabe.com</a>

---

Updated: {% include print_update.html %} • Like every project worth its salt, The Photographers Field Guide to Beijing needed its own style guide. I took my sticky notes and wrote this up for my editor. Maybe you'll find it useful, too.

## Mostly AP style?

Both the ebook and the mini site default to the **AP Style Guide** for spelling and punctuation. Yes, I _do_ know that it is obtuse at times. That's why:

* AP date format is annoying. Use MON DD YYYY instead. E.g. see "Updated: {% include print_update.html %}" at the top of this page.
* Numbers are never spelled out. Line-length is short, each character counts. Names might be an exception.
* Pinyin romanization is always used for Chinese words, names and places (see: Chinese).
* Ellipses are used as a narrative device (see: tone) – not to truncate quotes. Because this is not a newspaper…


## Styling content

### Chinese

Include hanzi alongside locations, names etc when it might help The Reader. Imagine just pointing to a map or word in the book to ask a cabbie or passerby for help. (Also see: [10 Assumptions.](https://www.zachmccabe.com/beijing/bts_10_assumptions.html))

### Oxford comma

The Oxford comma is not tolerated by AP Style, and this project is happy to abide by *that* rule.

### Photos

Photos need to support the copy, and, most of all, to tell a story.

### Reference books, tho

Reference books are typically considered boring, antiquated. Dirty little secret? This is a reference book – which means readers should be able to easily navigate info and hop back-and-forth without thinking about it. (Reference books are like an offline internet, which is perfect for travelers in China.)

### Small screens

Small screens are likely to be used by readers. It's a travel book after all. Write for mobile first. Keep paragraphs short, structure copy and visual queues to make reading in this environment easier.

### Spelling

Spelling is American English or Pinyin Chinese. Readership includes English speakers from _outside_ the US so it is important to be cognizant of these things. For the same reason, it is important to use standards of measure that are international.

(Beijingers will expect you not only to use the metric system, but also local standards like <mark>jin <span lang="zh">斤</span></mark> and <mark>wan <span lang="zh">万</span></mark>.)

### Tone

Tone should be personal and fun. Move it along because people need answers to their questions. They may already be on the ground. TBH try to go easy on the abbreviations, and for fuckssake don't say fuck. This book is meant for a wide-ish audience.



## Styling code

### Chunkify with headers, etc

Make the book easy to scan. (Also see: [10 Assumptions.](https://www.zachmccabe.com/beijing/10_assumptions.html)) Kindle puts some limits on how this is implemented. Use headers, short paragraphs, blockquote and and bold text to help chunkify information.


### Blockquote

Don't use blockquote for sidebars, info boxes or anything other than quotations. It's semantically incorrect (even if markdown makes it easy). To visually separate info for your reader, use `<span>` or `<div>` and a bit of CSS.

- Be careful with `<blockquote>` because Kindle appears to overrides your CSS. See: "Kindle CSS", below.
- Be careful with `<aside>` because iBooks is idiosyncratic about displaying contents wrapped in this tag. See: [Apple Books asset guide](https://help.apple.com/itc/booksassetguide/)


### Icons

All the old, inline icons were removed for the v2 field guide.

Iconography within the v1 field guide was in GIF format because, after much testing, Kindle's support for either PNG or SVG was a no go. Annoyingly there were _still_ some issues with the GIF files that made them distracting enough to limit their usefulness.

Lesson learned? Keep it simple, folks.


### Images

Within the ebook, images are 1:1 at 1000px. Photographs are JPG. Other visuals are PNG.


### Kindle CSS

In my testing, it seems like Kindle overrides CSS styling for many `html5` tags. I've had trouble with these:

* `<b>`
* `<blockquote>`
* `<figcaption>`
* `<h5>`
* `<h6>`
* `<mark>`
* `rgb() color` doesn't seem to work? I ran out of patience and stuck with hex. Be very careful with color in Kindle. There are usability issues, and possibly bugs.


### Line length

Line length can be a problem, watch out! Unfortunately, Kindle gives authors no control over presentation width. This can make reading feel breathless on narrower, mobile screens and exhausting on wider displays. (At least the reader has the option to dig into the settings and switch to a 2-column layout. How many readers know that option is there? How many toggle it on?) See also `Small screens`, under Content.


### Links

Be careful with links in the ebook. First, it annoyed beta readers to skip ahead and not be able to return to their previous location in the ebook. Second, external links to the web will likely be blocked by the GFW. Explain this, and use icons.

`<a href>` is old-fashioned, underlined and `#00f`. Within the book, this is important for any users with monochromatic e-ink Kindle devices. The mini site uses `#268bd2`, inspired by the always-stylish [Solarized](http://ethanschoonover.com/solarized).


### Multilingual

Multilingual words and phrases are noted with `<span>` tags and CSS. Chinese gets `<span lang="zh">` tags. Within a paragraph, the result looks like this: `<span class="hilite">English <span lang="zh">汉字</span></span>`. In the ebook, the `<mark>` tag is not used for this purpose because Kindle overrides custom CSS for this tag. Also, I wondered if `<mark>` might interfere with the user experience in both Kindle and some EPUB reader apps where Readers can highlight text?

On the mini site (like the rest of my website) I do use the `<mark>` tag and CSS to visually separate a multilingual span for The Reader, like this: <mark><span class="hilite">English <span lang="zh">汉字</span></mark>.
