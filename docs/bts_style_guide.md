---
layout: ratyear
date: 2017-12-05
update: 2020-02-10
title: Style guide
description: Style guide for The Photographers Field Guide to Beijing

---

Updated: {% include print_update.html %} • Like every project worth its salt, the field guide needed its own style guide. I took my sticky notes and organized them here. Maybe you'll find this useful, too.


## Mostly AP style?

Both the ebook and the mini site default to the **AP Style Guide** for spelling and punctuation. Yes, I _do_ know that it is obtuse at times. That's why I break some rules:

* AP date format is annoying. Use MON DD YYYY instead. E.g. see "Updated: {% include print_update.html %}" at the top of this page.
* Numbers are never spelled out. Line-length is short, each character counts. Names might be an exception.
* Pinyin romanization is always used for Chinese words, names and places. However, do not use tone marks because this isn't a text book (also see: Chinese).
* Ellipses are used as a narrative device – not just to truncate quotes. Because this is not a newspaper…


## Styling content

### Chinese

When it might help the reader, include hanzi alongside locations, names, etc. Imagine just pointing to a map or word in the book to ask a cabbie or passerby for help. (Also see: [10 Assumptions.](https://www.zachmccabe.com/beijing/bts_10_assumptions.html))

### Oxford comma

The Oxford comma is not tolerated by AP Style, and this project is happy to abide by *that* rule.

### Photos

Pictures should support the copy. Each additional picture adds weight to the ebook's file size on the readers device.

Most of all, each picture needs to tell a story.

### Reference books, tho

Reference books are typically considered boring. Dirty little secret? This is a reference book. And readers should be able to easily navigate info and hop back-and-forth without thinking about it.

(Reference books are like an offline internet. Perfect for travelers in China.)

### Small screens

Small screens are likely to be used by readers. It's a travel book after all. Write for mobile: Keep paragraphs short, structure copy and visual queues to make reading in this environment easier.

### Spelling

Spelling is American English or Pinyin Chinese. Readership includes English speakers from _outside_ the US so it is important to be cognizant of these things. For the same reason, it is important to use standards of measure that are international.

(Beijingers themselves will expect you not only to use the metric system but also local standards like <span class="hilite">jin <span lang="zh">斤</span></span> and <span class="hilite">wan <span lang="zh">万</span></span>.)

### Tone

Tone should be personal and fun.

Move it along because people need answers to their questions. The reader may already be on the ground.

TBH try to go easy on the abbreviations, and for fuckssake don't say fuck. This book is meant for a wide-ish audience.


### Quotes and citations

The AP stylebook is very clear *not* to use academic-style citations. That won't work for my purposes. Otherwise, I do try to follow the AP rules listed in "composition titles" and "quotations."

Long quotes should be used sparingly because this can disrupt reader's search for quick answers. Ideally, paraphrase. Link/HT as needed. Otherwise, try and limit supporting info, e.g. quotations, to footnotes for the curious reader.

- Web sources (social media, blogs, ebooks, whatever) should get a link back to the canonical source. 
- Citations that link to audio or video content should include a timestamp.
- Goals:
 + Citation info needs to be easy to scan for the reader; full Chicago citations can get very dense in this context it just looks silly.
 + Citations should be easy for me to format using markdown, which is the syntax I already use with the book and for the web.

Citations in the ebook, like the rest of my website, use a bastardized variant of Chicago.



## Styling code

### Chunkify with headers, etc

Make the book easy to scan. See: [10 Assumptions.](https://www.zachmccabe.com/beijing/10_assumptions.html)

Kindle puts some limits on how this is implemented. Use headers, short paragraphs, blockquote and bold text to help chunkify information.


### Blockquote

Don't use blockquote for sidebars, info boxes or anything other than quotations. It's semantically incorrect (even if markdown makes it easy). To visually separate info for the reader, use `<span>` or `<div>` and a bit of CSS.

- Be careful with `<blockquote>` because Kindle appears to overrides your CSS. See: "Kindle CSS", below.
- Be careful with `<aside>` because iBooks is idiosyncratic about displaying contents wrapped in this tag.

For more, see: [Apple Books asset guide](https://help.apple.com/itc/booksassetguide/)


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

Line length can be a problem, watch out! Unfortunately, Kindle gives authors no control over presentation width. This can make reading feel breathless on narrower, mobile screens and exhausting on wider displays. 

At least the reader has the option to dig into the settings and switch to a 2-column layout. (How many readers know that option is there? How many toggle it on?)

Also see: `small screens`.


### Links

Be careful with links in the ebook. First, it annoyed beta readers to skip ahead and not be able to return to their previous location in the ebook. Second, external links to the web will likely be blocked by the GFW. Explain this, and use icons.

`<a href>` is old-fashioned, underlined and `#00f`. Within the book, this is important for any users with monochromatic e-ink Kindle devices. The mini site uses `#268bd2`, inspired by the always-stylish [Solarized](http://ethanschoonover.com/solarized).


### Multilingual

Multilingual words and phrases are noted with `<span>` tags and CSS.

Chinese gets `<span lang="zh">` tags.

The result looks like this: `<span class="hilite">English <span lang="zh">汉字</span></span>`.

In the ebook, the `<mark>` tag is not used for this purpose because Kindle overrides custom CSS for this tag. Also, I wondered if `<mark>` might interfere with the user experience in both Kindle and some EPUB reader apps where readers can highlight text?
