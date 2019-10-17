---

layout: pek
pub-date: 2017-11-08
mod-date: 2018-04-15
title: How the book got made
image: https://www.zachmccabe.com/beijing/assets/viz/beijing-bonus-chapter-250.png
description: Here's how I put together my non-fiction book for Kindle. Wanna hint? Expect surprises…
lede: Here's how I put together my non-fiction book for Kindle. Wanna hint? Expect surprises…
cta: Support the project. Buy a copy of the <a href="https://www.amazon.com/Photographers-Field-Guide-Beijing-McCabe-ebook/dp/B072FVKP45/" alt="Get your copy on Amazon">book.</a> Karma will reward you with ice cream.

---


* [Photos](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#photos)
* [Maps and illustrations](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#maps-and-illustrations)
* [Copy](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#copy)
* [Kindle](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#kindle)
* [Lessons learned](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#lessons-learned)



### The long way

It would take extra work, I knew. This was my first book. From research, to draft and design, to marketing and shipping the final product, I wanted to be hands-on for the whole process. Trading efficiency for a fully DIY approach would give me important insight for the next book… Wouldn't it?

> Every project needs a [map](https://www.zachmccabe.com/beijing/bts_style_guide.html), a [compass](https://www.zachmccabe.com/beijing/bts_10_assumptions.html) and a soundtrack. I listened to [Halsey's cover](https://youtu.be/YIznx_ek98M) of "The Sound" about 5 thousand times.


### Photos

**Edit tight and compromise.**

When I started the book, I asked myself a question: _Does my reader even need to see the author's photos? After all, she's headed to Beijing to make her own._

This could be tested easily… In the first draft that went out to my beta readers the _only_ photo included in the Field Guide was on the cover. Reader response was unanimous: _"Where the hell are the photos, man?"_

The catch is that Kindle is not a charitable platform for any kind of images – and delivering high-quality photography to readers is especially troublesome.<sup><a id="ref1" href="#note1" alt="footnote">1</a></sup> Compare Kindle to Apple's iBooks: Amazon charges authors by file size, for one thing. The platform's code limits the responsive options we all take for granted with modern web browsers. And readers' devices run the gamut. (No more colorspace puns, I promise!)

It really isn't so bad though. The trick is rely on research and a solid user persona. Using these as my [map](https://www.zachmccabe.com/beijing/bts_style_guide.html) and [compass](https://www.zachmccabe.com/beijing/bts_10_assumptions.html), I knew what to do.

Each photo included in the Field Guide must:

1. Tell a good story.
2. Add context.
3. Avoid redundancy with the usual stuff (Instagram, tourist guidebooks).
4. Reinforce the tone and message of the Field Guide.

With the help of my photo editor, 11 photos, each 1500 px with a 1:1 ratio, were included in the Field Guide. Files weighed between 220 - 500 kb when uploaded to Amazon. Because I wanted to give Amazon's own compression algorithms as much data to work with as possible, I didn't compress the JPGs at all.

> Monochrome images were chosen for the vibe, not for potential weight-savings. Sure didn't hurt.


#### Not so picture perfect

We're used to the experience delivered by modern web browsers. Compared to looking at photos using a web browser, in Kindle, neither the author or the reader have much control. Expectations for the Field Guide were high, regardless.

Research told me many photographers are very choosy about their displays – my images would need to meet the demands of top-shelf phones and tablets.<sup><a id="ref2" href="#note2" alt="footnote">2</a></sup>

But device storage space is truly at a premium during international trips.

An ebook like mine would be competing for space alongside movies for the flight, other ebooks and travel apps, and, most importantly for photographers, copies of their own images. It is easy to imagine a Reader backing up her photos to an iPad. She might also proof those images with an app like Lightroom, too.

So I was much less concerned about showing off high-quality images in the book than I was with the risk of taking up space on Readers' devices. Then there is that irritable warning from Kindle to customers: _"Due to its large file size, this book may take longer to download."_ I assume I'm not the only one who tries to download just-one-more before it's time to get on the plane? I also [assume](https://www.zachmccabe.com/beijing/bts_10_assumptions.html) that some of my Readers are in scenarios where network connectivity isn't great.

According to the Amazon product page, the Field Guide weighs 7978 KB. This is roughly the same file size as a hefty novel or nonfiction book – like Michael Meyer's great book, [Last Days of Old Beijing.](https://www.amazon.com/Last-Days-Old-Beijing-Backstreets-ebook/dp/B003WUYE3E/)

Book | Published file size
--- | ---
Photographers Field Guide |7978 KB
Lonely Planet Beijing | 86787 KB
Last Days of Old Beijing | 7559 KB


### Maps and illustrations

**If you can't get there, you probably can't photograph it.**

Offline maps weren't part of the plan, at first. _If most readers will be reading the Field Guide on their phone, won't they just reach for their favorite maps app?_

As research progressed I realized that I'd need to include custom maps for 3 reasons. Feedback from early readers convinced me that:

1. Few travelers are willing to endure the extra hassles caused by the GFW to get to that favorite maps app.
2. Although there are very good English-language maps designed for tourists, there were still large info gaps.
3. Maps are an efficient, quick way to organize and explain complex ideas – making them an ideal way to deliver info to [my reader](https://www.zachmccabe.com/beijing/bts_10_assumptions#the-ebook). 

By the time the dust settled, I'd decided to include 14 maps alongside the 17 illustrations I'd already made.

Both the maps and other illustrations were created in SVG. Start with Joni Trythall's [Pocket Guide to Writing SVG](http://svgpocketguide.com/book/). It is brilliant, and I only wish I'd found it sooner.

Maps were illustrated using [Maperative](http://maperitive.net/) on top of open-source [OSM data](http://www.openstreetmap.org/about). Some hand-polishing of the raw XML and the output SVG files was needed. Maperative is a brilliant tool although it takes some extra work to get it up and running on MacOS. (Anyway, none of the other options I found provided cost-effective licensing for ebooks.)

Other illustrations were just coded by hand in [BBEdit](https://www.barebones.com/products/bbedit/).


#### SVG GIF JPG wtf

Creating these visuals was the most challenging part of getting the Field Guide published.

Early tests revealed that, in fact, Kindle's SVG support was too limited. Thanks to [Image Magick](https://www.imagemagick.org/script/index.php) and [Inkscape](https://inkscape.org/en/), I was able to get everything translated to GIF.<sup><a id="ref3" href="#note3" alt="footnote">3</a></sup>  Finally, everything was put through [ImageOptim](https://imageoptim.com/mac) to compress the files down as small as possible.

Because it was the first time I'd done something like this, the workflow and technical challenges were beastly. It took significantly _more_ time to complete than actually writing and editing the copy. 

Worth it? Absolutely. So far nobody has said a thing – which means the visuals are doing their job.


### Copy

**Writing a book is hard enough, so I try to keep my tools simple and streamlined.**

My earliest drafts were puked out in MacOS' **TextEdit**. Inevitably my best ideas were noted on-the-go with whatever was handy on my phone, including **Evernote** and  video selfies.

All this was assembled into a working draft. However, beta testers pointed out the structure of the book wasn't practical. _They were right._ Between the revisions and what was thrown out, I ended up rewriting the whole Field Guide. It was for the best.

As the project developed, I needed some structure. [Gitbook](https://www.gitbook.com/) allowed me to pull my disparate TXT files together. Writing in Markdown is great, so that's what I did. Being able to easily add my visuals, and edit captions and other bits alongside the rest of the copy in Gitbook was awesome.


#### Writing for mobile

Assuming that most readers would be paging through the Field Guide on their phones, I wrote for _that_. It took some practice. I reread the [usual sources](https://ux.stackexchange.com/questions/108801/what-is-the-best-number-of-paragraph-width-for-readability).

The [AP Stylebook](https://www.zachmccabe.com/beijing/bts_style_guide.html) might be Religion, but the good book provides no advice on typefaces, [line length](http://maxdesign.com.au/articles/em/) or other UI issues. I dove a little too happily into arcane studies.

The most useful resources were [Butterick](https://practicaltypography.com/line-length.html) and the [BBC](http://www.bbc.co.uk/academy/journalism/skills/digital-journalism/article/art20141202144618106).

Unfortunately, Kindle gives authors very little control over UI, and no control over presentation [width.](https://baymard.com/blog/line-length-readability) This can make reading feel breathless on narrower, mobile screens and exhausting on wider displays. (At least the reader has the option to dig into the settings and switch to a 2-column layout. How many readers know that option is there? How many toggle it on?)


### Kindle

**Designing and coding for Kindle is not the same as a webpage, it turns out.**

Since I wrote in **Gitbook**, it was easy to export the whole thing as an EPUB. The output was alright. Anyway, I still needed to get some things worked out in the XHTML files for specifically for Kindle. Paul Salvette's [books](http://bbebooksthailand.com/) were an awesome resource for understanding what needed to be done. **BBEdit** and [Calibre](https://calibre-ebook.com/) got me the rest of the way there.


### Lessons learned

**If you're making a product you will have to experiment, test and revise. Recruit your team early on.**

The Field Guide is the first book I've written. It's not the first book I've helped produce, though. It's also not my first big, hairy project. 

There were a few false summits that caught me by surprise. I took some wrong turns. Again, I'd like to emphasize the importance of having a compass – you need to create a reader persona and learn to consult that document as part of your process. Mine is [here.](https://www.zachmccabe.com/beijing/bts_10_assumptions.html)

Find your beta testers (beta readers?) as soon as you can. Treat their time with respect. This feedback is invaluable.

Then, find a good editor. If you're including maps, illustrations and photos, pull in a photo editor or a designer, too. These eagle-eyed folks will catch mistakes and help guide you through the 11th-hour gales.

I was told to spend half my time making the product and half my time marketing it. I should've listened.

From the start I knew I wanted to do the whole thing myself. I wanted to understand how it works. It really was worth the extra effort, confusion and truly sickening number of late nights.

I'm pulling together a team for the next book. If you're interested, <a href="mailto:hello@zachmccabe.com">let me know.</a>


### Notes

<h4 id="note1">Note 1</h4>

There are several challenges with photos and visual content – and Amazon itself isn't always the limiting factor:

**Compression.** Kindle automatically compresses images and the rest of the content you upload. This is probably in everyone's best interest. The scant documentation on images doesn't serve readers or authors well.

**Resolution and colorspace.** Mobile devices can be among the most demanding ways to view an image. That said, a 500 ppi mobile display and an e-ink reader with limited processing power want very different things from a photograph. Both Kindle gurus and the platform's own documentation advise authors to consider their readers' needs. Good advice!  

**Grayscale, btw.** Kindle documention doesn't mention which grayscale conversion standard they utilize (or if it's proprietary, which some authors have asserted). I can only say that it's worth testing your color illustrations on Amazon's own e-ink hardware. <a href="#ref1" alt="back">↩</a>

<h4 id="note2">Note 2</h4>

[DPI.lv](http://dpi.lv/) helped me get a better idea of my reader's resolution needs. Then it was time to experiment. Like the rest of the content, photos were tested on half a dozen different devices. Then I solicited feedback (and screenshots) from beta testers. <a href="#ref2" alt="back">↩</a>

<h4 id="note3">Note 3</h4>

ImageMagick's great `convert` command let me quickly transform SVGs to GIFs. However, it did have some trouble with the bilingual copy on my maps.

I needed all the visuals to look consistent, and styled the text with a generic `font-family="sans-serif"`. But ImageMagick stumbled with Chinese fonts. The program outputted Chinese text in serifed type, even though it outputted English text in the sans-serif I expected. As I couldn't find a remedy, the SVG maps were converted to GIF using Inkscape instead. <a href="#ref3" alt="back">↩</a>
