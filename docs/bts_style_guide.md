---

layout: pek
pub-date: 2017-12-05
mod-date: 2018-04-06
title: Style guide
description: Like every project worth its salt, The Photographers Field Guide to Beijing needed its own style guide...
lede: I took my sticky notes and wrote this up for my editor. Maybe you'll find it useful, too.
cta: Support the project. Buy a copy of the <a href="https://www.amazon.com/Photographers-Field-Guide-Beijing-McCabe-ebook/dp/B072FVKP45/" alt="Get your copy on Amazon">book.</a> Karma will reward you with ice cream.

---

### Mostly AP style?

Both the ebook and the mini site default to the **AP Style Guide** for spelling and punctuation. Yes, I _do_ know that it is obtuse at times. That's why:

* AP date format is annoying. Use YYYY-MM-DD instead. E.g. "page last updated." 
* Numbers are never spelled out. Line-length is short, each character counts. Names might be an exception.
* Pinyin romanization is always used for Chinese words, names and places (see: Chinese).
* Ellipses are used as a narrative device (see: tone) – not to truncate quotes. Because this is not a newspaper…


### Styling content

#### Chinese

Include hanzi alongside locations, names etc when it might help The Reader. Imagine just pointing to a map or word in the book to ask a cabbie or passerby for help. (Also see: [10 Assumptions.](https://www.zachmccabe.com/beijing/bts_10_assumptions.html))

#### Oxford comma

The Oxford comma is not tolerated by AP Style, and this project is happy to abide by *that* rule.

#### Photos

Photos need to support the copy, and, most of all, to tell a story.

#### Reference books, tho

Reference books are typically considered boring, antiquated. Dirty little secret? This is a reference book – which means readers should be able to easily navigate info and hop back-and-forth without thinking about it. (Reference books are like an offline internet, which is perfect for travelers in China.)

#### Small screens

Small screens are likely to be used by readers. It's a travel book after all. Write for mobile first. Keep paragraphs short, structure copy and visual queues to make reading in this environment easier.

#### Spelling

Spelling is American English or Pinyin Chinese. Readership includes English speakers from _outside_ the US so it is important to be cognizant of these things. For the same reason, it is important to use standards of measure that are international.

(Beijingers will expect you not only to use the metric system, but also local standards like <mark>jin <span lang="zh">斤</span></mark> and <mark>wan <span lang="zh">万</span></mark>.)

#### Tone

Tone is personal, fun. Move it along because people need answers to their questions. They may already be on the ground. TBH try to go easy on the abbreviations, and for fuckssake don't say `fuck`. This book is meant for a wide-ish audience. 


### Styling code

Within the ebook itself, `<h1>` is used for sections, i.e. `Sections 1 - 3, Resources and Locations Appendix`. The mini site doesn't use `<h2>` tags but the ebook uses them for chapter headings. In the ebook both `<h1>` and `<h2>` get forced page breaks.

#### Chunkify with headers, etc

Make the book easy to scan. (Also see: [10 Assumptions.](https://www.zachmccabe.com/beijing/10_assumptions.html)) Kindle puts some limits on how this is implemented. Use headers, short paragraphs, blockquote and and bold text to help chunkify information.

Note `<h5>` or `<h6>` are used to emphasize a point. `#ff5c5c` on the mini site, only. Unlike other headers, they're always used as a complete sentence. (Within the ebook, `<b>` is used instead because Kindle CSS wasn't cooperative.)

#### Blockquote

Blockquote is used to add a personal note to an idea, to annotate or further explain the main idea. In the current iteration of the ebook, don't use `<blockquote>`. Instead, use `<span>` because Kindle CSS doesn't like it.

> Example blockquote. Markdown means that I'm using `blockquote` instead of `aside`.


#### Icons

Iconography within the ebook is in `.gif` format because, after much testing, Kindle's support for either `.png` or `.svg` is a no go. Annoyingly there are still some major issues with the `.gif` files in the ebook, and they'll be killed in the next update.

#### Images

Images are kept to a minimum for speedy load times on the mini site. Screenshots and explanatory visuals are in color and typically just `.png` files; photographs are `.jpg` files and are monochromatic both in the ebook and on the mini site. (For the nitty gritty on image processing workflow, dimensions, classes, etc, and when to use what… check the `readme`.)


<figure>
  <img class="vizdot" src="https://www.zachmccabe.com/beijing/assets/viz/proof/this-cat-500.jpg" alt="requisite example cat" />
  <figcaption>
    <p>Image caption looks like this. Note the requisite Example Cat, above.</p>
  </figcaption>
</figure>


#### Kindle CSS

It's worth noting here that, in my testing, seems like Kindle doesn't support CSS styling for many `html5` tags. I've had trouble with these:

* `<b>`
* `<blockquote>`
* `<figcaption>`
* `<h5>`
* `<h6>`
* `<mark>`
* `rgb() color` doesn't seem to work, I ran out of patience and stuck with hex. Be very careful with color in Kindle. There are usability issues, and possibly bugs.

#### Line length

Line length can be a problem, watch out! Unfortunately, Kindle gives authors no control over presentation width. This can make reading feel breathless on narrower, mobile screens and exhausting on wider displays. (At least the reader has the option to dig into the settings and switch to a 2-column layout. How many readers know that option is there? How many toggle it on?) See also `Small screens`, under Content.

#### Links

Be careful with links in the ebook. First, it annoyed beta readers to skip ahead and not be able to return to their previous location in the ebook. Second, external links to the web will likely be blocked by the GFW. Explain this, and use icons.

`<a href>` is old-fashioned, underlined and `#00f`. Within the book, this is important for any users with monochromatic e-ink Kindle devices. The mini site uses a stylish `#268bd2`, thanks to [Solarized](http://ethanschoonover.com/solarized).

#### Multilingual
Multilingual words and phrases are noted with `<mark>` tags. Chinese gets `<span lang="zh">` tags. Within a paragraph, the result looks like this: `<mark>English <span lang="zh">汉字</span></mark>`.


### Lessons learned

For v1.2 I guess the ebook will need `class="EvenMoreClasses"`. Maybe if I properly markup the mini site and manuscript, I can just search and replace? 😭
