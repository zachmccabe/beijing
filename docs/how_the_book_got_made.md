---
layout: ratyear
pub-date: 2017-11-08
mod-date: 2020-01-30
title: How the book got made
image: https://www.zachmccabe.com/beijing/assets/viz/beijing-bonus-chapter-250.png
description: Here's how I put together my non-fiction book for Kindle. Wanna hint? Expect surprises…
cta: Your feedback on methods, tools and – of course – the field guide itself is always welcome. Let me know what you think. <a href="mailto:hello@zachmccabe.com">hello@zachmccabe.com</a>

---


*Updated: Jan 31 2020.* For the 3rd time in >5 years, I've rewritten the field guide.

It's like bouncing along in a noisy, old carriage on the overnight train – the bed under you rattles wildy enough that your sleep is anxious.

Is it weird that I find the rhythm comforting anyway?


- v2.0.0: Jan 2020, published via free ePub and on Kindle
- v1.0.0: May 2017, published on Amazon Kindle
- v0.0.0: Oct 2016, unpublished
- Research begins in early 2015


Thankfully, only 1 brave soul had to endure that very first iteration. (And I'm thankful he did! His feedback convinced me that the book would need to be reorganized. At that point, I also ripped out much of the exsisting copy and started writing again.)



* [The long way](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#the-long-way)
* [Map and compass](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#map-and-compass)
* [Photos](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#photos)
* [Maps and illustrations](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#maps-and-illustrations)
* [Copy](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#copy)
* [Writing for mobile](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#writing-for-mobile)
* [Lessons learned](https://www.zachmccabe.com/beijing/how_the_book_got_made.html#lessons-learned)



## The long way

It would take extra work, I knew. This was my first book. From research, to draft and design, to marketing and shipping the final product, I wanted to be hands-on for the whole process. Trading efficiency for a fully DIY approach would give me important insight for the next book… Wouldn't it?


## Map and compass
Every project needs a [map](https://www.zachmccabe.com/beijing/bts_style_guide.html), a [compass](https://www.zachmccabe.com/beijing/bts_10_assumptions.html) and a soundtrack. I listened to [Halsey's cover](https://youtu.be/YIznx_ek98M) of "The Sound" on BBC Radio 1 about 5k times.

All of my decisions are made using that [map](https://www.zachmccabe.com/beijing/bts_style_guide.html) and [compass.](https://www.zachmccabe.com/beijing/bts_10_assumptions.html) Reader feedback, and input from comrades who've generously helped me edit the copy and pictures in the book, have helped me refine those tools.


## Photos

**Edit tight and compromise.**

Each photo included in the Field Guide must:

1. Tell a good story.
2. Add context.
3. Avoid redundancy with the usual stuff (Instagram, tourist guidebooks).
4. Reinforce the tone and message of the Field Guide.

When I started the book, I asked myself a question: _Does my reader even need to see the author's photos? After all, she's headed to Beijing to make her own._

Test it! In the beta that went out to a hardy group of testers (readers?), the only photo included in the Field Guide was on the cover. Reader response was unanimous: _"Where the hell are the photos, man?"_



### Version 2

All photos are 1000px with a 1:1 ratio.

This update includes 3x more photos. The choice seemed straight forward: nearly everyone complained about the lack of pictures in the previous version.

While v1 only included monochrome images (which were chosen to reinforce the contrarian vibe of the book), I decided to ditch that approach this time because it wasn't working for my readers.


Amazon v1 | Amazon v2 | EPUB v2
--- | --- | ---  
11 photos | 37 photos | 37 photos
7978 KB* | 13537 KB* | 9360 KB†

*According to the Amazon product pages.\
†According to my Github repo.


As you can see in the table above, the EPUB weighs less than the Amazon version, which is interesting because Amazon *starts* with that same EPUB file. 

Amazon, iBooks and other platforms request authors upload "original, high resolution" files. (There are some good reasons to request this. There are also some sloppy reasons to request this.) Because I'm now distributing the field guide on Amazon and also directly as an ePub, I optimized image files myself before before packing them. I need to keep my workflow streamlined:

1. Keep photo dimensions "small," at 1000px 1:1. Again, navigating with my map and compass.
2. Compress image files using [ImageOptim.](https://imageoptim.com/mac)
3. Pack these files and build the EPUB file. (That EPUB is uploaded to my Github repo, and also converted to MOBI and uploaded to Amazon.)






### Version 1

Eleven photos, each 1500 px with a 1:1 ratio, were included in the v1 field guide. Files weighed between 220 - 500 kb when uploaded to Amazon. Because I wanted to give Amazon's own compression algorithms as much data to work with as possible, I didn't compress the JPGs at all.


### More notes from V1: picture perfect

Kindle is not a charitable platform for any kind of images – and delivering high-quality photography to readers is especially troublesome.<sup><a id="ref1" href="#note1" alt="footnote">1</a></sup> Compare Kindle to Apple's iBooks: Amazon charges authors by file size, for one thing. The platform's code limits the responsive options we all take for granted with modern web browsers. And readers' devices run the gamut. (No more colorspace puns, I promise!)

Compared to looking at photos using a web browser, in Kindle, neither the author or the reader have much control. Expectations for the Field Guide were high, regardless.

Research told me many photographers are very choosy about their displays – my images would need to meet the demands of top-shelf phones and tablets.<sup><a id="ref2" href="#note2" alt="footnote">2</a></sup>

But device storage space is truly at a premium during international trips.

An ebook like mine would be competing for space alongside movies for the flight, other ebooks and travel apps, and, most importantly for photographers, copies of their own images. It is easy to imagine a Reader backing up her photos to an iPad. She might also proof those images with an app like Lightroom, too.

So, I was much less concerned about showing off high-quality images in the book than I was with the risk of taking up space on Readers' devices. Then there is that irritable warning from Kindle to customers: _"Due to its large file size, this book may take longer to download."_

- I assume I'm not the only one who tries to download just-one-more before it's time to get on the plane?
- I also [assume](https://www.zachmccabe.com/beijing/bts_10_assumptions.html) that some of my Readers are in scenarios where network connectivity isn't great.

According to the Amazon product page, the v1 field guide weighed 7978 KB. This is roughly the same file size as a hefty novel or nonfiction book – like Michael Meyer's great book, "Last Days of Old Beijing."

Book | Published file size
--- | ---
Photographers Field Guide v1 | 7978 KB
Lonely Planet Beijing | 86787 KB
Last Days of Old Beijing | 7559 KB




## Maps and illustrations

**If you can't get there, you probably can't photograph it.**

Offline maps weren't part of the plan, at first. _If most readers will be reading the Field Guide on their phone, won't they just reach for their favorite maps app?_

As research progressed I realized that I'd need to include custom maps for 3 reasons. Feedback from early readers convinced me that:

1. Few travelers are willing to endure the extra hassles caused by the GFW to get to that favorite maps app.
2. Although there are very good English-language maps designed for tourists, there were still large info gaps.
3. Maps are an efficient, quick way to organize and explain complex ideas – making them an ideal way to deliver info to [my reader](https://www.zachmccabe.com/beijing/bts_10_assumptions#the-ebook). 

In the v1 field guide, I included 14 high-level, thumbnail maps alongside the 17 illustrations I'd already made. (Some of these were removed from the v2 field guide.)

Both the maps and other illustrations were created in SVG.

Joni Trythall's [Pocket Guide to Writing SVG](http://svgpocketguide.com/book/) is brilliant, and I only wish I'd found it sooner.

Maps were illustrated using [Maperative](http://maperitive.net/) on top of open-source [OSM data](http://www.openstreetmap.org/about). Some hand-polishing of the raw XML and the output SVG files was needed. Maperative is a brilliant tool although it takes some extra work to get it up and running on MacOS. 

Anyway, none of the other options I found provided cost-effective licensing for ebooks.

Other illustrations were just coded by hand in [BBEdit](https://www.barebones.com/products/bbedit/).



### SVG GIF JPG wtf

**Reality is not spec. Face palm.**


- Photographers Field Guide v2: Assuming enough time has past that it's safe to go with PNG.
- Photographers Field Guide v1: All non-photo assets were translated to GIF for max backwards compatibility.

Originally, all the maps and illustrations in the v1 field guide were to be published in SVG. According to both the ePub spec and Amazon's spec for their own formats, SVG should've worked. Reality is not spec. Early tests (2016) revealed that, in fact, Kindle's SVG support was too limited. 

At that point I also learned that, apparently, some of Amazon's e-ink hardware couldn't render PNG. In the v1 field guide, it looked like my only options were JPG for photos, and GIF<sup><a id="ref3" href="#note3" alt="footnote">3</a></sup> for everything else.

**ImageOptim** was used to compress the files down as small as possible.

Creating the illustrations and thumbnail maps was certainly the most challenging part of the v1 field guide. Because it was the first time I'd done something like this, the workflow and technical challenges were beastly. It took significantly _more_ time to complete than actually writing and editing the copy. 

Worth it? <strike>Absolutely. So far nobody has said a thing – which means the visuals are doing their job.</strike> You tell me: <hello@zachmccabe.com>.



## Copy

**Writing a book will tucker you out, so I try to keep my tools simple and streamlined.**


### Version 2

Gitbook changed their product offering, and wasn't used in this version.

Everything was written in Markdown, using **TextEdit.** Then, using [Pandoc,](https://pandoc.org/) I built a rough ePub. This was hand polished with [Calibre](https://calibre-ebook.com/) and **BBEdit.**

All are excellent tools. Calibre is very useful for editing and debugging ePub files. Pandoc can be used for all sorts of things. Both have active communities. If you're trying to build a book, try them out.



### Version 1

My earliest drafts were puked out in MacOS' **TextEdit**. Inevitably my best ideas were noted on-the-go with whatever was handy on my phone, including **Evernote** and  video selfies. This mess was then assembled into a working draft.

As the project developed, I needed more structure. [Gitbook](https://www.gitbook.com/) allowed me to pull my disparate TXT files together. Writing in Markdown is great, so that's what I did. Being able to easily add my visuals, and edit captions and other bits alongside the rest of the copy in Gitbook was very helpful.

From Gitbook, it was easy to export the whole thing as an EPUB. The output was alright. Anyway, I still needed to get some things worked out in the XHTML files specifically for Kindle. Paul Salvette's [books](http://bbebooksthailand.com/) were an awesome resource for understanding what needed to be done. **BBEdit** and [Calibre](https://calibre-ebook.com/) got me the rest of the way there.



## Writing for mobile

Presentation [width](https://baymard.com/blog/line-length-readability) is critically important to the readability with any text.


- On narrow phone screens, short lines of text feel breathless.
- On wider screens, long lines of text are fatiguing.


Some apps/platforms do a better job of helping Readers understand they can tweak UI options (e.g. line height, columns, font choice).

Presentation will continue to be a challenge for authors of digital books, web pages and any other situation where content flows to fit in un-fixed containers. It seems to me that this is simply a natural characteristic of this medium.

Assuming that most Readers would be paging through the field guide on their phones, I wrote for _that_. It took some practice. I reread the [usual sources](https://ux.stackexchange.com/questions/108801/what-is-the-best-number-of-paragraph-width-for-readability).

The [AP Stylebook](https://www.zachmccabe.com/beijing/bts_style_guide.html) might be Religion, but the good book provides no advice on typefaces, [line length](http://maxdesign.com.au/articles/em/) or other UI issues. More useful:

- [Butterick](https://practicaltypography.com/line-length.html)
-  And the [BBC](http://www.bbc.co.uk/academy/journalism/skills/digital-journalism/article/art20141202144618106).


For the v2 field guide, I needed to step back and reorganize the book's structure once again. Abby Covert's book, ["How to make sense of any mess"](http://www.howtomakesenseofanymess.com/) and Craig Mod's [essays](https://craigmod.com/essays/to_make_a_book_walk_on_a_book/) were very helpful.



## Lessons learned

**If you're making a product you will have to experiment, test and revise. Recruit your team early on.**

The Photographers Field Guide to Beijing is the first book I've written. It's not the first book I've helped produce, though. It's also not my first big, hairy project. 

Nevertheless, there were a few false summits that caught me by surprise. I took some wrong turns. Again, I'd like to emphasize the importance of having a compass – you need to create a reader persona and learn to consult that document as part of your process. Mine is [here.](https://www.zachmccabe.com/beijing/bts_10_assumptions.html)

1. Find your beta testers (beta readers?) as soon as you can. Treat their time with respect. This feedback is invaluable.
2. Then, find a good editor. If you're including maps, illustrations and photos, pull in a photo editor or a designer, too. These eagle-eyed folks will catch mistakes and help you through the 11th-hour gales.
3. I was told to spend half my time making the product and half my time marketing it. I should've listened.

From the start I knew I wanted to do the whole thing myself. I wanted to understand how it works. It really was worth the extra effort, confusion and truly sickening number of late nights.

Make a book. You'll be happy you did.



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
