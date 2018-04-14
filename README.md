# My Recurse Center Syllabus

```
            o                   o
             \               __/
              \___          /
                  \__    __/
                     \  /
 ____________________\/_________________
/   _________________________________   \
|  /__/  \__  _____________ \__/  \__\  |
| |    __   \____My_________    __   \| |
| |\__/  \_________________ \__/  \__ | |
| |    __   \___Recurse_____    __   \| |
| |\__/  \__  _____________ \__/  \__ | |
| |    __   \_______Center__    __   \| |
| |\__/  \__  _____________ \__/  \__ | |
| |    __   \__Syllabus____     __   \| |
| |\__/  \__  _____________ \__/  \__ | |
|  \________\________________________/  |
|                                       |
|                          _   _   _    |
|  Ashley Blewer!         (=) (=) (=)   |
\______________________________________/
     "--"                      "--"
 ```

# Creating a syllabus for myself 

I will be attending the [Recurse Center](https://recurse.com) from April 2 until June 28. For the uninundated (non-inundated?), I have been describing RC succinctly as "like a writer's retreat for programmers." although maybe that's not quite sufficient. But in general, it is a place to focus intensely on my craft and be surrounded by and inspired by brilliant people.

I am [verrrrrry excited](https://twitter.com/ablwr/status/963424473725767681)!

Because the time you spend at RC and what you choose to work on is self-initiated and self-motivated, I am setting up this repository to create a sort of "syllabus" for myself and what I want to accomplish. **BUT! I do not expect to follow it, just give myself some rough structure to make sure I hit my personal productivity goals while leaving enough room for unanticipated discovery.**

**This will also be a living syllabus,**   
updated with links to blog posts,   
works I produced,   
and things I used to tackle these problems  
or build things for each week.

Some things will get bumped and other things will get shuffled around as part of the normal un-learning process.

**Here is how I answered the application question "What would you like to work on at the Recurse Center?":**

I really love video and I understand it (relatively) well, I think, but would really like to better understand compression algorithms and how things work. I think trying to make my own video codec would be a good way to do that, and RC seems like a great place to attempt a task that sounds difficult and academic. I think this kind of broad, open-ended task would allow me to have one major goal to accomplish, and would allow me to break down the problem and potentially tackle mini-problems along the way, accepting productive distraction (like committing to an open source video framework as a mini-goal towards the larger educational goal).


**General suggestions from RC to help think about projects:**

* What are the main 2-3 things I'd like to learn? (i.e. why am I doing this?)  
* Which features could I build to learn them?  
* Are there other things I can ignore because they won't help me achieve my learning goals?  
* Does my project divide naturally into certain chunks?  
* How will I know when my project is finished?  


**Thinking about how to think about this**

I want to create goals for myself that are concrete enough to be able to tackle but open enough that I can move in different directions as I grow and learn more. 

I also think it's important for me to think about this work as at *most* 80% of a week, leaving 20% to spread out and learn about or engage in other projects unrelated to this one. But I hope that for each week, I can formulate an idea of readings/tasks to complete, and ensure a solid balance of learning-time and active-programming time.


# Week 0 (Now until April 2)

Create this syllabus. 

Here are some things inspiring me (and related to this topic):

- [Falsehoods Programmers Believe about Video](https://haasn.xyz/posts/2016-12-25-falsehoods-programmers-believe-about-%5Bvideo-stuff%5D.html)
- [Vittorio Giovara - Color Me Intrigued: A Jaunt Through Color Technology in Video](https://www.youtube.com/watch?v=XMnvY7a4-As)
- [Vittorio Giovara - Introduction to video reverse engineering](https://vimeo.com/158036897)
- [Digital Video and HD: Algorithms and Interfaces by Charles Poynton](https://www.goodreads.com/book/show/431195.Digital_Video_and_HD)
- [http://www.memo.tv/learning-to-see-you-are-what-you-see/](http://www.memo.tv/learning-to-see-you-are-what-you-see/)
- [Data compression paper](https://github.com/papers-we-love/papers-we-love/blob/master/data_compression/data-compression.pdf)
- [Pirate TV](http://www.instructables.com/id/How-To-Save-Analog-TV/)
- [Kieran O'Leary - Learning Through Fixity Errors](https://kieranjol.wordpress.com/2018/03/29/learning-through-fixity-errors/)

Popular algorithm names:
- Huffman 
- Adaptive Huffman!
- Shannon-Fano
- Schwartz-Kallick

## (Pre-RC Ideas Zone, this will move)
- Video container/codec review, how do significant properties relate to each other when established by each format?
- containers versus codecs, how do they work together (or not together?)
- Begin manipulation of raw video data 
- "signal processing"
- Muxing, demuxing, compiling code  
- ffmpeg filters
- Visualizing compression: Is there a way to extract only-the-compression from audio or video for visualization purposes? 
- Build something in C -> I did build something in Rust with much help, so maybe this has been satisfied
- Colorspaces
- Subtitles 
- Codec manipulation
- Web Assembly, put C in the browser 
- Electron, put JS on the desktop
- Thinking about open source contributions here



# Week 1 (April 2-6): "Containers/codecs"

## Code written 

- Hmm, nothing that would merit a check-in...

## Exploring Matroska attachments
- file format polyglot-ing (put mkv file inside mkv file)
- This was very easy thanks to [MKVToolNix](http://mkvtoolnix.download/)!  
- **BLOG POST** [Making a Matroska Magic Hat](http://bits.ashleyblewer.com/blog/2018/04/02/matroska-magic-hat/).

## Understand how codecs are made 
- **BLOG POST** [All the stuff between EBML and Matroska](http://bits.ashleyblewer.com/blog/2018/04/03/all-the-stuff-between-ebml-and-matroska/)
- **BLOG POST** [Exploring codecs and data streams](http://bits.ashleyblewer.com/blog/2018/04/03/exploring-codecs-and-data-streams/)
- read up on codecs

## Open or non-open codecs, standards:

- [ffv1](https://github.com/FFmpeg/FFV1)
- [lenticular](https://github.com/amiaopensource/lenticular) by reto kromer
- [openjpeg](https://github.com/uclouvain/openjpeg)
- [RTP Payload Format for H.264 Video](https://tools.ietf.org/html/rfc6184)
- [AV1](https://aomedia.org/av1-bitstream-and-decoding-process-specification/)
- [Daala](https://xiph.org/daala/)
- Not open: [h.264](https://en.wikipedia.org/wiki/H.264/MPEG-4_AVC)
- Not open: [ProRes white paper](https://www.apple.com/final-cut-pro/docs/Apple_ProRes_White_Paper.pdf)
- Not open: [ProRes RAW white paper](https://images.apple.com/final-cut-pro/docs/Apple_ProRes_RAW_White_Paper.pdf)

## ffmpeg! 

- FFmpeg has been coming up a lot in conversation, with a lot of people working on different things. Someone told me about [this book](https://www.amazon.com/FFmpeg-Basics-Multimedia-handling-encoder/dp/1479327832) which is like the best thing ever. I'm ready to start a graduate level program and teach only this book. So many example commands and a visual representation of what they do.
- I need to follow advice that Misty De Meo was given and passed along via Mastodon, which is "hacking around some stuff in FFmpeg's encoder to see what happens"
- Misty's Sega FILM demuxer is in ffmpeg now [github](https://github.com/FFmpeg/FFmpeg/commit/187ff5a10864f16b7872eca722e844e8f04ec57b) and I'm #fangirling 

## Codec exploration: ./lenticular 

- **BLOG POST** [Lenticular film, lenticular codec](http://bits.ashleyblewer.com/blog/2018/04/04/lenticular-film-lenticular-codec/)
- investigation of [lenticular](https://github.com/amiaopensource/lenticular), a codec-in-progress for lenticular film
- Running lenticular partially successfully 
- Ran into [segmentation faults](https://en.wikipedia.org/wiki/Segmentation_fault) and I'd like to explore these more, but moving on for now

## File formats, methods of implementation 

- deep read: [the secret life of nan](https://anniecherkaev.com/the-secret-life-of-nan). This blog post casually mentions standardization drama and I clicked on the link to read more SO fast. It's [here](https://people.eecs.berkeley.edu/~wkahan/ieee754status/754story.html)
- deep read: [google docs, not a file format](https://madfileformatscience.garymcgath.com/2018/03/15/google-docs/) I like these two quotes in a succinct blog post: "Proprietary formats are always risky. When the format isn’t a file format at all, you can’t even reverse-engineer it in principle." and "Don’t be a cheapskate. Pay for the storage you need."
- deep read: [How can we preserve Google Documents?](https://digital-archiving.blogspot.co.uk/2017/04/how-can-we-preserve-google-documents.html)

## gdb / debugging in C 

- `brew install gdb` 
- [extra stuff for macOS](https://stackoverflow.com/questions/18423124/please-check-gdb-is-codesigned-see-taskgated8-how-to-get-gdb-installed-w)
- Is the problem: macOS, gcc, gdb, Homebrew, XCode, the code, or something else?
- "Reading symbols from lenticular...(no debugging symbols found)...done."
- "Undefined symbols for architecture x86_64" - sometimes this is macOS being weird, but sometimes this is just me not remembering to call an external lib in C
- "duplicate symbol \_main in:"" - added -c to the two .o rules to tell gcc to stop at the compilation stage. But also noting that this could be main being defined twice in the program.
- My brain today: "How do you debug a debugger?"
- [Valgrind](http://valgrind.org/)
- `brew install valgrind`

## Rust 

- [rustup](https://www.rustup.rs/)
- [roundup of learning resources](https://github.com/ctjhoa/rust-learning)
- [Docs v2](https://doc.rust-lang.org/book/second-edition/)
- [playing in browser](https://play.rust-lang.org/)
- I like that the compiler tells you when something is unused
- `cargo build` to compile your crate
- `cargo run` to run it
- "statements (executing code), ... expressions (returning a value)."

## Manipulating data 
- ❣️ Pairing with Casey on building a simple image manipulation script in Rust 
- ❣️ [Data Compressor From Scratch](https://www.destroyallsoftware.com/screencasts/catalog/data-compressor-from-scratch)

## gpg/pgp
- Intro from Ernest 
- pki, public key infrastructure
- "web of trust" / "strong set"
- expiration and revokation 
- "security convenience balance"
- yubikey is closed source, nitrokey is open software/hardware 
- Ring (end to end encrypted Skype) ring.cx

## Cultural heritage and copyleft opinions 

Lots of talks and inspiration from batchmate [Marianne](http://mkcor.github.io/):  
- http://ivory.idyll.org/blog/2017-digital-commons-funding.html paper about CC models   
- ❣️ https://framagit.org/mkcor/free-software-ethics Marianne's talk on free software ethics, so so so so good!
- "pragmatic idealism"   
- deep read: Potential video cultural heritage paper to read (and maybe love?): https://hal-mines-paristech.archives-ouvertes.fr/hal-00975857v2/document  
- "Intangible Cultural Heritage"
- TIL: "apt-get install [anarchism](https://packages.debian.org/source/stretch/anarchism)" installs [this](https://theanarchistlibrary.org/library/the-anarchist-faq-editorial-collective-an-anarchist-faq)

## Preservation of complex media
- [Re-Collection: Art, New Media, and Social Memory](http://re-collection.net/educational_resources.html)
- ❣️ "variable media behaviors": contained, installed, performed, interactive, reproduced, interchangeable, encoded, networked
- wishing I could play [this interactive fiction on laserdisk](https://digipres.club/@joe/99814029127707315)

## Feelings 
- **BLOG POST** [First Week at Recurse Center](http://bits.ashleyblewer.com/blog/2018/04/06/first-week-at-RC/).
- Something obvious to me when working in the context of the humanities is that we each have specific knowledge about a subject derived from our own lenses and cumulative individual experience (hello Black feminist critical theory), and the sooner I acknowledge this applies to technical subjects too, the better off I’ll be. RC is a great place for this because of the diverse experience and backgrounds collaborating in one space, but harder in a small monoculture like digital preservation.
- adding increasingly dangerous amounts of coffee, trying to reign it in

## Misc 
- first added a xml feed to my blog, next day I actually showcase that endpoint so people can use it: http://bits.ashleyblewer.com/feed.xml if you want to subscribe
- TIL zulip offers free hosting for OSS projects https://zulipchat.com/for/open-source/
- more zulip love: you can view source, you write in markdown 
- Looking at http://www.vapoursynth.com/about/
- [my review was requested](https://github.com/amiaopensource/audiorecorder/pull/69) on audiorecorder
- "are you upstate or something? I picture you in some sort of compound like the end of mad men"
- YCbCr: "But how do you make yellow?" Because colorspaces are cubes, and the absence of blue produces yellow, and the absence of red produces green.
- fell into the same Jekyll time zone trap as Marianne did this week: A few of my posts was originally written at something like "23:16:00 -0400" so when the time changed for daylight savings, it reverted to thinking it "should" be the next day, deleting the original page and replacing it with a date that was one day later. Tricky! My hack to resolve it was to not get so granular with time-of-posts and kept it at the day-level for these late-ish night additions. 
- Lydia recommends: https://www.goodreads.com/book/show/44882.Code



# Week 2 (April 9-13): "Minimum Viable Codec"

## Code written 
- [menstruation rollercoaster (2D)](http://bits.ashleyblewer.com/menstruation-dataviz/): ya my period data from the last decade is irregular.

## Minimum Viable Codec
- What does this look like?

## Rust vs multimedia 
- **BLOG POST** [Considering Rust](http://bits.ashleyblewer.com/blog/2018/04/09/considering-rust/)
- **BLOG POST** [Considering Rust ...for Video](http://bits.ashleyblewer.com/blog/2018/04/10/considering-rust-for-video/)
- [Kostya's Boring Codec World](https://codecs.multimedia.cx/)
- but especially: [NihAV — Concept and Principles](https://codecs.multimedia.cx/2017/06/nihav-concept-and-principles/)
- The above blog post helps me break down my own problems-I-will-be-creating-for-myself with this statement: "I hope the domain for NihAV is clear: it will take ByteIO input, demux data using it (packets or elementary stream chunks—if you want them in packet format then use a parser), optionally fill timestamp information, decode frames, reorder them in display order if requested, similar approach for writing data."
- [Huffman coding implementation in Rust](http://pramode.in/2016/09/26/huffman-coding-in-rust/)

## Rust in general
- **BLOG POST** [Error Handling in Rust](http://bits.ashleyblewer.com/blog/2018/04/12/error-handling-in-rust/)
- **BLOG POST** [Stealing Snax using Rust](http://bits.ashleyblewer.com/blog/2018/04/13/stealing-snax-using-rust/)
- ["How to rewrite your project in Rust"](https://unhandledexpression.com/2017/07/12/how-to-rewrite-you-project-in-rust/)
- [nom](https://github.com/Geal/nom)
- Something I won't be doing soon PROBABLY, making [a N64 emulator in rust](https://www.youtube.com/playlist?list=PL-sXmdrqqYYcznDg4xwAJWQgNL2gRray2)
- ❣️ [Rust Cookbook](https://rust-lang-nursery.github.io/rust-cookbook/intro.html)
- ❣️ [rustlings](https://github.com/carols10cents/rustlings): Small exercises to get you used to reading and writing Rust code. SUPER SMALL! Really excited about the simplicity here and it pushed me to really read [the book](https://doc.rust-lang.org/book/second-edition/ch01-00-introduction.html), which is also full of examples.


## rust-av
- [Luca Barbato: Rust-av: Rust and Multimedia](https://blogs.gentoo.org/lu_zero/2018/02/14/rust-av-rust-and-multimedia/)
- ❣️ [Introducing rust-av, A pure-Rust approach to multimedia](https://fosdem.org/2018/schedule/event/rust_av/) video from FOSDEM '18, also the "slides" used in this presentation are amazing
- ❣️ [rust-av github](https://github.com/rust-av/rust-av)

## Codecs, etc

- [HuffYUV](https://wiki.multimedia.cx/index.php?title=HuffYUV)
- [Chroma from Luma Intra Prediction for AV1](https://docs.google.com/presentation/d/13yUG1lyNmf_TtWARvOJRGa05EVknKya-VEDZ_8L22P8/edit#slide=id.p)
- [Chroma from Luma lightning talk](https://bambuser.com/v/6909221#t=7258s): intra-frame! Video from VDD '17
- [CfL Design Doc for AV1 (draft)](https://docs.google.com/document/d/1T86spqQqt7o3LWj3FeaOPUJ2vZ_DSgImJ2r0on8wP-g/edit)
- [Data Compression Conference Proceedings](http://www.cs.brandeis.edu/~dcc/Program.html)
- [Fast Averaging of High Color (16 bit) Pixels](https://medium.com/@luc.trudeau/fast-averaging-of-high-color-16-bit-pixels-cb4ac7fd1488)
- [Videos about AV1](https://www.youtube.com/watch?v=68uCu-jWbgU&list=PLDa6QBb3vqVzcVBCWS3WKrcvf4ZqJeiW-)

## Video, in general 

- ["How VLC works"](http://dev.unhandledexpression.com/slides/rustconf-2016/vlc/#17.0): a helpful slide!
- ["Multimedia Data"](http://users.cs.cf.ac.uk/Dave.Marshall/Multimedia/node141.html)
- "data moshing" but actually doing it instead of just "enjoying" it 
- ❣️ [Irish Film Archives great microservices collection](https://github.com/kieranjol/IFIscripts)
- [What Is A LUT? Explained with Cats.](https://vimeo.com/120318153)

## Linear Algebra 

I think I may have to overcome my utter lack of maths knowledge soon...
- above is clearly everything I'm doing to avoid this topic
- [Matrix coefficient](https://en.wikipedia.org/wiki/Matrix_coefficient)?
- [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) (thanks Jess!)
- [New fast.ai course: Computational Linear Algebra](http://www.fast.ai/2017/07/17/num-lin-alg/) (thanks Jess!)

## Feelings

- **BLOG POST** [Second Week at RC](http://bits.ashleyblewer.com/blog/2018/04/13/second-week-at-RC/)
- Learning can feel painful and that's okay! 
- How to make mistakes, acknowledge them, correct them, and move forward.
- The difficulties of committing (and wanting to commit) to 100% focus on something (this) but still having to manage winding down paused or ending freelance projects, maintaining pre-existing relationships, and trying not to worry about housing and employment after RC.

## Misc 
- [aparrish/text-resources](https://github.com/aparrish/text-resources)
- TIL: `| hexdump` does exactly what you think it does
- [destroyallsoftware: intro to computation series](https://www.destroyallsoftware.com/screencasts/catalog/introduction-to-computation)
- wondering why I didn't learn how to use Vim 3 years ago 🙄 because it's great 😅
- bonus [vimrc](https://github.com/amix/vimrc)
- I made kombucha for the first time, it was rose flavored, and I drank it.
- Play all these at the same time: [1](https://www.youtube.com/watch?v=FSxquE6VDiQ), [2](https://www.youtube.com/watch?v=OwLq7Q4J5tw), [3](https://www.youtube.com/watch?v=XBcWAydqtow)
- [Rosa Menkman - A Vernacular of File Formats](https://www.slideshare.net/r00s/rosa-menkman-a-vernacular-of-file-formats-4923967)


# Week 3 (April 16-20)


# Week 4 (April 23-27)


# Week 5 (April 30 - May 4)


# Week 6 (May 7-11)

- Codec-building! rough drafts?

# BONUS WEEK (May 14-18)

[!!Con May 12-13](http://bangbangcon.com/) - I got a ticket!

This is when Never Graduate Week happens. SPRING BREAKKKKKKKK!

# Week 7 (May 21-25)

- Codec-building, codec-built? 

# Week 8 (May 28 - June 1)

- Codec-building, codec-built? 

# Week 9 (June 4-8)

- Steps to build a video player?

# Week 10 (June 11-15)

[ TBD: Intentionally unstructured play ]

# Week 11 (June 18-22)

[ TBD: Intentionally unstructured play ]

# Week 12 (June 25-28)

[ TBD: Intentionally unstructured play ]

# THE END!  

There is no end! Never graduate!

# Mini-projects

Some ideas I have for small projects to work on!

## Birthday-starmap generator
 
Generate an image that shows the state of the solar system at the time of someone's birth and text that explains how that aligns to someone's astrological sign (and moon sign, and rising sign). I think this mini-project will involve: Understanding the rules of astrology, some math about how fast planets move around the sun in relation to each other, ImageMagick to produce a proper image.

## Significant contribution(s) to Audiorecorder

[Audiorecorder](https://github.com/amiaopensource/audiorecorder) is a small, simple audio digitization command-line tool that has recently pushed up a new GUI made in Shoes (Ruby). It can use some help in making the application run a little bit better using this new framework.

## Recreating computer/video art in CSS or Processing.js

Learn how to better use Processing, new CSS features, or new HTML5 features by recreating early computer/video artworks. lillian schwartz, vera molnar, ken knowlton, john whitney, manfred mohr, dara birnbaum, paul sharits, hollis frampton, michael snow, nam june paik, stan vanderbeek are all potential artists to be inspired by and whose work I can attempt to replicate. I think this may involve some math.

## Linter?

Write a linter? A few starting links:
https://stackoverflow.com/questions/70705/how-to-write-a-linter  
https://github.com/mcandre/linters  

## "Long Time Vine Preservation"

Fulfill a long-running joke with a friend of mine.