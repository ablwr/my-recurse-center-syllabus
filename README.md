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

## Blogging 

- [Making a Matroska Magic Hat](http://bits.ashleyblewer.com/blog/2018/04/02/matroska-magic-hat/).
- [All the stuff between EBML and Matroska](http://bits.ashleyblewer.com/blog/2018/04/03/all-the-stuff-between-ebml-and-matroska/)
- [Exploring codecs and data streams](http://bits.ashleyblewer.com/blog/2018/04/03/exploring-codecs-and-data-streams/)
- [Lenticular film, lenticular codec](http://bits.ashleyblewer.com/blog/2018/04/04/lenticular-film-lenticular-codec/)
- [First Week at Recurse Center](http://bits.ashleyblewer.com/blog/2018/04/06/first-week-at-RC/).

## Exploring Matroska attachments
- file format polyglot-ing (put mkv file inside mkv file)
- This was very easy thanks to [MKVToolNix](http://mkvtoolnix.download/)!  

## Understand how codecs are made 
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



# Week 2 (April 9-13): R U S T

## Code written 
- [menstruation rollercoaster (2D)](http://bits.ashleyblewer.com/menstruation-dataviz/): ya my period data from the last decade is irregular.
- [Internet Girlfriend Club Volume 7 goes live](http://internetgirlfriend.club/)

## Blogging 
- [Considering Rust](http://bits.ashleyblewer.com/blog/2018/04/09/considering-rust/)
- [Considering Rust ...for Video](http://bits.ashleyblewer.com/blog/2018/04/10/considering-rust-for-video/)
- [Error Handling in Rust](http://bits.ashleyblewer.com/blog/2018/04/12/error-handling-in-rust/)
- [Stealing Snax using Rust](http://bits.ashleyblewer.com/blog/2018/04/13/stealing-snax-using-rust/)
- [Second Week at RC](http://bits.ashleyblewer.com/blog/2018/04/13/second-week-at-RC/)

## Minimum Viable Codec
- What does this look like?

## Rust vs multimedia 
- [Kostya's Boring Codec World](https://codecs.multimedia.cx/)
- but especially: [NihAV — Concept and Principles](https://codecs.multimedia.cx/2017/06/nihav-concept-and-principles/)
- The above blog post helps me break down my own problems-I-will-be-creating-for-myself with this statement: "I hope the domain for NihAV is clear: it will take ByteIO input, demux data using it (packets or elementary stream chunks—if you want them in packet format then use a parser), optionally fill timestamp information, decode frames, reorder them in display order if requested, similar approach for writing data."
- [Huffman coding implementation in Rust](http://pramode.in/2016/09/26/huffman-coding-in-rust/)

## Rust in general
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


# Week 3 (April 16-20) "Minimum Viable Codec" (Encoding)

## Code written
- [hello264-rust](https://github.com/ablwr/hello264-rust)
- [avpres-training: video update](http://training.ashleyblewer.com/presentations/video.html)
- [ablwr/talks/ARCH2018](https://github.com/ablwr/talks)
- [ffmprovisr](https://github.com/amiaopensource/ffmprovisr): open/close all recipe syntax and new recipe

## Blogging 
- [Week 3 Feelings Check-in](http://bits.ashleyblewer.com/blog/2018/04/21/third-week-at-recurse-center-feelings-check-in/)
- [What is a Minimum Viable Codec?](http://bits.ashleyblewer.com/blog/2018/04/21/what-is-a-minimum-viable-codec/)

## Analog Video! 
- [Tektronix - The Vectorscope -- It's All About Color! V 2.0](https://www.youtube.com/watch?v=z-UBLJdd2g0)
- [Understanding Analog Video Signals](https://www.maximintegrated.com/en/app-notes/index.mvp/id/1184)
- [Video format tables](http://videopreservation.conservation-us.org/dig_mig/video_formats_v4_850.html)
- [New York City in 1993 in HD - DTheater DVHS Demo Tape](https://www.youtube.com/watch?v=fT4lDU-QLUY) | [theverge writup](https://www.theverge.com/2016/4/25/11503816/new-york-city-hd-footage-manhattan)
- "cost of action calculator"

## Encoding 
- ❣️ [World's Smallest h.264 Encoder](https://cardinalpeak.com/blog/worlds-smallest-h-264-encoder/)
- [Minimal video player example](http://roxlu.com/2014/039/decoding-h264-and-yuv420p-playback) (h264 decoder!)
- [The h.264 Sequence Parameter Set](https://cardinalpeak.com/blog/the-h-264-sequence-parameter-set/)
- [Common Intermediate Format](https://en.wikipedia.org/wiki/Common_Intermediate_Format)

## Rust 
- [intermezzOS](https://intermezzos.github.io/)
- [How Rust Do](https://blog.jfo.click/how-rust-do/) (some wav generation knowledge here)

## Misc 
- Teaching in DC on Tues - Sad to miss even one day 😿
- TIL: `vimtutor`
- Analyze [moshbot](https://github.com/lirien/moshbot)
- TIL: `| nc termbin.com 9999` for quick code-sharing between computers
- [trackingjs](https://trackingjs.com/)
- [Essential thoughtleadership theory](https://www.youtube.com/watch?v=AqSZhwu1Rwo)
- [Software Defined Radio hardware](https://www.amazon.com/gp/product/B011HVUEME/ref=od_aui_detailpages00?ie=UTF8&psc=1)
- TIL: `xxd` looks better (imo) than `hexdump`
- [h264bitstream](https://github.com/aizvorski/h264bitstream) command-line tool to read/write h264 bitstreams
- [C Syntax cheatsheet](https://courses.cs.washington.edu/courses/cse351/14sp/sections/1/Cheatsheet-c.pdf)


# Week 4 (April 23-27) "Minimum Viable Codec" (Decoding)

## Goals 
Goals at the start of this week:  
- Writing h264 decoder / mini-player 
- Getting Rust to the browser with wasm - done!
- Writing encoder for video streams using huffman algo
- Not have a cold anymore - done!

## Code written 
- Hmmm...

## Blogging 
- [Uncompressed versus uncompressed packed video](http://bits.ashleyblewer.com/blog/2018/04/25/uncompressed-versus-uncompressed-packed-video/)
- [What does audiovisual compression look like?](http://bits.ashleyblewer.com/blog/2018/04/26/what-does-audiovisual-compression-look-like/)
- [Rust Study Group Notes](http://bits.ashleyblewer.com/blog/2018/04/27/rust-study-group-notes/)
- [Week 4 of 12 at Recurse Center](http://bits.ashleyblewer.com/blog/2018/04/27/week-four-at-recurse-center/)

## WASM 
- [Hello wasm-pack!](https://hacks.mozilla.org/2018/04/hello-wasm-pack/)
- [Significance of documentation in rating Rust crates](http://rust-lang.github.io/rfcs/1824-crates.io-default-ranking.html#easy-to-use)

## Video 
- ❣️ [Introducing AV1 and Open Video Codecs](https://www.youtube.com/watch?v=lEdqN22vaWs)
- [four.cc: YUV Pixel Formats](http://www.fourcc.org/yuv.php)
- [four.cc: YUV to RGB Conversion](http://www.fourcc.org/fccyvrgb.php)
- "linesize"??
- [frei0r filters](https://frei0r.dyne.org/)
- `ffplay -f lavfi mptestsrc=t=all`
- [Current Status of Codecs in Nov 2017 talk](https://www.streamingtech.se/player.html?id=stswe17-ozer): Has me thinking about the massive costs associated with license-based codecs, really drives home how important the open collaborative work of AV1. Also thinking about how codecs are geographically-based in significance when these licensing/royalties costs to decode or for hardware-support are involved.
- "Same quality" -- how is quality assessed?
- `-psy               <boolean>    E..V..... Use psychovisual optimizations. (default auto)` (sounds cooler than it is)
- [Streaming Video and Audio with Low Delay](http://steinwurf.com/blog/2018-04-25-2022.html)
- ❣️ [Learn FFmpeg libav the Hard Way](https://github.com/leandromoreira/ffmpeg-libav-tutorial#learn-ffmpeg-libav-the-hard-way)
- [vaporwave player](https://github.com/bdon/vaporwave)
- "transrating" changing the bitrate of a file 

## Deep video 
- [deepfakes/faceswap](https://github.com/deepfakes/faceswap): ostensibly more trustworthy source code
- [df](https://github.com/dfaker/df): for making corpus
- [Exploring deepfakes](https://hackernoon.com/exploring-deepfakes-20c9947c22d9)
- [The Era of Fake Video Begins](https://www.theatlantic.com/magazine/archive/2018/05/realitys-end/556877/)
- [Tensorflow tutorials](https://www.tensorflow.org/tutorials/)
- [Introduction to Deepfakes tutorial series](https://www.alanzucconi.com/2018/03/14/introduction-to-deepfakes/)


## Misc 
- "computer mediated mysticism"
- [zodiacpress](https://github.com/isabelc/zodiacpress) for the technical underpinning of how astrological natal charts are created and here's an [example](https://cafeastrology.com/free-natal-chart-report.html) in case I want to rewrite
- "wholesome deepfakes"
- ["What does it mean to raise a family or to grow up under constant surveillance?"](http://www.nybooks.com/daily/2018/04/21/the-fbis-vulgar-betrayal-of-muslim-americans/)
- Something to think about later: [TLA+](https://en.wikipedia.org/wiki/TLA%2B)
- [mosh_bot source code](https://github.com/lirien/moshbot)
- [Delta.NYC](https://www.civichalllabs.org/probonotech/)
- "side data" and "main data"
- "bit reservoir"
- "syntactic noise"
- how the internet works outside of home router
- "smart pointers"
- [Cinder](https://libcinder.org/)
- [3d snorlax](https://www.thingiverse.com/thing:2264822)
- [Theorizing the Web 2018](http://theorizingtheweb.org/ttw18/)

YUV2RGB shader math  
```
vec3 yuv = vec3(yColor.r - 16.0/256, uColor.r - 0.5, vColor.r - 0.5);
oColor.x = dot(yuv, vec3(1.164,  0.000,  1.596));
oColor.y = dot(yuv, vec3(1.164, -0.391, -0.813));
oColor.z = dot(yuv, vec3(1.164,  2.018,  0.000));
```

# Week 5 (April 30 - May 4) (Floating in space)

## Code written 
- [pbcore-validator](http://bits.ashleyblewer.com/pbcore-validator/)
- [uninsured body simulator](https://github.com/ablwr/uninsured): moles, ocular migraines
- [where all the planets at?](https://github.com/ablwr/planets)

## Blogging 
- [The Story of Goldilocks and the Three WebAssembly Libraries](http://bits.ashleyblewer.com/blog/2018/05/03/goldilocks-and-the-three-webassembly-libraries/)
- [Week 5 at Recurse Center](http://bits.ashleyblewer.com/blog/2018/05/04/week-five-at-recurse-center/)
- [Mapping the planets with Rust+WebAssembly+JavaScript+Canvas](http://bits.ashleyblewer.com//blog/2018/05/05/mapping-the-planets/)

## Calling C in Rust 
- [Foreign Function Interface](https://doc.rust-lang.org/nomicon/ffi.html)
- [Calling a C function from Rust](https://blog.jfo.click/calling-a-c-function-from-rust/)
- [Calling C from Rust](https://jvns.ca/blog/2016/01/18/calling-c-from-rust/)

## A return to Rust+WASM+JS
- [JavaScript to Rust and Back Again: A wasm-bindgen Tale](https://hacks.mozilla.org/2018/04/javascript-to-rust-and-back-again-a-wasm-bindgen-tale/)
- [Parc3l: Combining Three.js, Rust, and WebAssembly!](https://medium.com/@cwervo/parc3l-combining-three-js-rust-and-webassembly-c1e643ef7681)

## Video 
- [DASH playback of AV1 video in Firefox](https://hacks.mozilla.org/2017/11/dash-playback-of-av1-video/)
- [VLC sample files](http://streams.videolan.org/samples/)

## Video players
- [Glide media player](https://crates.io/crates/glide)
- [h264-live-player](https://github.com/131/h264-live-player)
- [Broadway](https://github.com/mbebenita/Broadway)
- [ogv.js](https://github.com/brion/ogv.js/)
- [web-dsp](https://github.com/shamadee/web-dsp)

## Misc 
- [How does Chromaprint work](https://oxygene.sk/2011/01/how-does-chromaprint-work/)


# Week 6 (May 7-11) (Planets in alignment)

## Code written 
- [Talk: Internet Girlfriend Club!](https://github.com/ablwr/talks)
- [planets](http://bits.ashleyblewer.com/planets/), updated with opts and deployed

## Blogging 

## Malaysian General Election 2018 
- [Malaysian General Election c/o Wikipedia](https://en.wikipedia.org/wiki/Malaysian_general_election,_2018)
- Batchmate [Janice Shiu's story](https://www.facebook.com/partitur/posts/10156008545400399)

## Video 
- [ffmpeg in the browser!!!!!!! videoconverter.js demo](https://bgrins.github.io/videoconverter.js/demo/)
- [ffmpeg.js](https://github.com/Kagami/ffmpeg.js)
- [Building ffmpeg.js for Ubuntu](https://paul.kinlan.me/building-ffmpeg.js/)
- [Decode it like its 1999](http://phoboslab.org/log/2017/02/decode-it-like-its-1999)
- [Engineers Making Movies (AKA Open Source Test Content)](https://medium.com/netflix-techblog/engineers-making-movies-aka-open-source-test-content-f21363ea3781)

## Misc 
- ashleyblewer.com finally went https!
- [XPADxpert](https://www.basicmaster.de/xpadxpert/)
- [Resisting Surveillance: it's is not just about the metadata](https://media.ccc.de/v/camp2015-6741-resisting_surveillance_it_s_is_not_just_about_the_metadata#t=3601)
- [MENSTRUAPPS – How to turn your period into money (for others)](https://chupadados.codingrights.org/en/menstruapps-como-transformar-sua-menstruacao-em-dinheiro-para-os-outros/)
- [Servo engine](https://research.mozilla.org/servo-engines/)
- [Aura reading](https://www.refinery29.com/aura-reading)
- [American Mall Game](https://www.bloomberg.com/features/american-mall-game/)
- Spending most of my time prioritizing being around people who are leaving this week

# BONUS WEEK (May 14-18)

[!!Con May 12-13](http://bangbangcon.com/) - I got a ticket!

This is when Never Graduate Week happens. SPRING BREAKKKKKKKK!

## Code written 
- [I-Ching](http://bits.ashleyblewer.com/i-ching/#x1101x) gets a save-state upgrade and makeover

# Week 7 (May 21-25) (Reboot)

## Code written 
- X 

## Blogging 
- X 

## Back 2 video 
- [AV1 Bitstream & Decoding Process Specification](https://aomediacodec.github.io/av1-spec/av1-spec.pdf)

## Manipulating video in the browser 
- [webgazer.js](https://webgazer.cs.brown.edu/)
- [canvasfilters](https://github.com/kig/canvasfilters)
- [Manipulating video using canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Manipulating_video_using_canvas)

## Deepfakes again
- [Family fun with deepfakes. Or how I got my wife onto the Tonight Show](https://towardsdatascience.com/family-fun-with-deepfakes-or-how-i-got-my-wife-onto-the-tonight-show-a4454775c011)

## MATH 
- [Beautiful linear algebra videos](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
- [Computer color is broken](https://www.youtube.com/watch?v=LKnqECcg6Gw)

## Misc 
- [the cryptopals crypto challenges](https://cryptopals.com/)
- [ProofMode](https://blog.witness.org/2017/07/media-activists-witness-guardian-project-back/) adds encrypted chunk of data to media
- [Is This For Real? How InformaCam Improves Verification of Mobile Media Files](https://blog.witness.org/2013/01/how-informacam-improves-verification-of-mobile-media-files/)
- tfw you get disheartened because you don't realize you're trying to solve an outstanding research problem
- "Here, we introduce a framework in which we quantify these perceptual distortions in terms of “just intolerable differences” (JIDs)."
- [violent-theremin](https://github.com/mdn/violent-theremin)


# Week 8 (May 28 - June 1)

## Code written
- [more-blue](https://github.com/ablwr/more-blue): another very tiny codec

## Blogging 
- [Weeks 7 and 8 at Recurse Center](https://bits.ashleyblewer.com/blog/2018/05/28/weeks-7-and-8-at-recurse-center/)

## Encoding 
- [rav1e - av1 encoder in rust](https://github.com/xiph/rav1e)
- OBU = Open Bitstream Unit
- [YUV4MPEG2 (.y4m) Encoder/Decoder Crate](https://crates.io/crates/y4m)
- ["Category:Undiscovered Video Codecs"](https://wiki.multimedia.cx/index.php/Category:Undiscovered_Video_Codecs)
- [S268M_Revised](http://www.simplesystems.org/users/bfriesen/dpx/S268M_Revised.pdf)
- closed standards are immoral

## Rust
- [RustFest Paris 2018 video playlist](https://www.youtube.com/watch?v=23lRkdDXqY0&list=PL85XCvVPmGQgdqz9kz6qH3SI_hp7Zb4s1)
- "[Redox](https://www.redox-os.org/) is a Unix-like Operating System written in Rust, aiming to bring the innovations of Rust to a modern microkernel and full set of applications."

## Misc 
- [DEF CON 25 - Svea Eckert, Andreas Dewes - Dark Data](https://www.youtube.com/watch?v=1nvYGi7-Lxo)
- [DEF CON 25 - Matt Wixey - See no evil, hear no evil: Hacking invisibly & silently with light & sound](https://www.youtube.com/watch?v=gFTiD7EnVjU&list=PL9fPq3eQfaaDOo8mTBHhEHMfuG2LNUSTC&index=65)
- [Tactical Tech Collective](https://tacticaltech.org/)
- [Efficiency and Madness - Using Data and Technology to Solve Social, Environmental and Political Problems](https://www.boell.de/en/2017/11/28/efficiency-and-madness-using-data-and-technologyto-solve-social-environmental-and-political-problems)
- [Ray Tracer #1: What is a ray tracer?](https://www.youtube.com/watch?v=RIgc5J_ZGu8)
- [conrod](https://github.com/PistonDevelopers/conrod): "An easy-to-use, 2D GUI library written entirely in Rust."

YUV - RGB Conversion  
```
R = Y + 1.4075 * (V - 128)
G = Y - 0.3455 * (U - 128) - (0.7169 * (V - 128))
B = Y + 1.7790 * (U - 128)

Y = R *  .299000 + G *  .587000 + B *  .114000
U = R * -.168736 + G * -.331264 + B *  .500000 + 128
V = R *  .500000 + G * -.418688 + B * -.081312 + 128
```

# Week 9 (June 4-8)

## Code written

## Blogging 

## Real Life Hour 
- returning from [DC](https://upload.wikimedia.org/wikipedia/commons/2/26/The_Library_of_Congress%2C_Washington-LCCN2008678216.jpg), going to [Boston](https://twitter.com/BostonJoeSly/status/319604880044077056)
- [e-slow-tion](https://www.youtube.com/watch?v=tnR1jmuqdJo&list=PLaLEOGfFWw_tWsxqHhblGYxf5OuKS_GrT&index=1)

## Rust 
- [gotham.rs](https://gotham.rs/)
- [The Secret Life of Cows](https://deterministic.space/secret-life-of-cows.html)

## Video 
- [Comparing video codecs and containers for archives](http://download.das-werkstatt.com/pb/mthk/info/video/comparison_video_codecs_containers.html)
- [Digital intermediate](https://en.wikipedia.org/wiki/Digital_intermediate)
- [Sustainability of Digital Formats: Digital Moving-Picture Exchange (DPX), Version 2.0](https://www.loc.gov/preservation/digital/formats/fdd/fdd000178.shtml)
- [Sustainability of Digital Formats: Digital Video Encoding (DV, DVCAM, DVCPRO)](https://www.loc.gov/preservation/digital/formats/fdd/fdd000183.shtml)
- [Misinterpreting Mandelbrot](https://www.youtube.com/watch?v=_s7JsWeUSRo)
- [Xiph.org test media](http://media.xiph.org/)

## Misc 
- [A Framework For Purposeful Open Source](https://medium.com/mozilla-open-innovation/whats-your-open-source-strategy-here-are-10-answers-383221b3f9d3)
- [Project Electron Update: Introducing Aurora 1.0](http://blog.rockarch.org/?p=1997)
- [Bit Manipulation](https://www.hackerearth.com/practice/notes/bit-manipulation/)

# Week 10 (June 11-15) 🎊🎂🆎

## Video Pixel Formats
- I feel like I should be thinking about pixel formats more. 
- [Microsoft: Pixel Formats for Uncompressed Video](https://docs.microsoft.com/en-us/windows-hardware/drivers/display/pixel-formats-for-uncompressed-video)
- [Apple: Core Video - Available Pixel Formats](https://developer.apple.com/library/archive/qa/qa1501/_index.html)


## Misc 
- [Localhost: Samantha Goldstein Crafting a Connected Home](https://www.recurse.com/events/localhost-samantha-goldstein)
- [Critical .zip vulnerabilities?](https://www.youtube.com/watch?v=Ry_yb5Oipq0)
- [edX Introduction to Linux](https://courses.edx.org/courses/course-v1:LinuxFoundationX+LFS101x+1T2017/course/)
- [The Land Before Binary](https://medium.com/@bellmar/the-land-before-binary-cc705d5bdd70)
- [About Time: Sifting Through Analog Video Terminology](https://patchbay.tech/2018/06/11/about-time/)
- feeling 😵😵😵

# Week 11 (June 18-22) ⿒

## Blogging 

- [Weeks 9, 10, 11 at Recurse Center](https://bits.ashleyblewer.com/blog/2018/06/23/weeks-9-10-11-at-recurse-center/)

## Python 
- getting my env un-fucked 
- [The key differences between Python 2.7.x and Python 3.x with examples](http://sebastianraschka.com/Articles/2014_python_2_3_key_diff.html)
- [conda](https://conda.io/docs/)
- [pipenv](https://github.com/pypa/pipenv)


## Misc 
- [returning to fish](https://fishshell.com/docs/current/index.html)
- [The Book of Shaders](https://thebookofshaders.com/)
- [OIL OF EVERY PEARL'S UN-INSIDES](https://www.youtube.com/watch?v=AC8h4HnWyys)
- [x86 assembly doesn’t have to be scary (interactive)](https://blog.benjojo.co.uk/post/interactive-x86-bootloader-tutorial)
- [Overscripted! Digging into JavaScript execution at scale](https://hacks.mozilla.org/2018/06/overscripted-digging-into-javascript-execution-at-scale/)
- [Explainer on Sigfried, FIDO, and DROID matching differences](http://openpreservation.org/blog/2014/09/27/siegfried-pronom-based-file-format-identification-tool/)
- [Resurrecting the first Dutch web index: NL-menu revisited](http://openpreservation.org/blog/2018/04/24/resurrecting-the-first-dutch-web-index-nl-menu-revisited/)
- [How I use Wireshark](https://jvns.ca/blog/2018/06/19/what-i-use-wireshark-for/)
- [Princeton Web Transparency & Accountability Project](https://webtap.princeton.edu/)
- [What's going on up the street?](https://motherboard.vice.com/en_us/article/xwmpm7/ways-your-city-is-surveilling-you-police-government-surveillance)

# Week 12 (June 25-28) 🙀

## Python
- [ipdb](https://pypi.org/project/ipdb/)
- [Problem Solving with Algorithms and Data Structures using Python](http://interactivepython.org/runestone/static/pythonds/index.html)

## Back on my bullshit
- [OSSArcFlow](https://educopia.org/research/ossarcflow)
- "The Innovation Interest Group is no longer active."
- [Genesis of a File Format](http://exponentialdecay.co.uk/blog/genesis-of-a-file-format/)

## AV1
- [AOM AV1 codec mapping in Matroska/WebM draft](https://github.com/Matroska-Org/matroska-specification/blob/av1-mappin/codec/av1.md)
- [av1 1.0.0](https://aomedia.googlesource.com/aom/+/v1.0.0)

## scanlime video content 
- [Little Glitchy CRT](https://www.youtube.com/watch?v=v3u74DmISpc)
- [Little live teardown of NTSC test pattern Tek](https://www.youtube.com/watch?v=3rBf_p6mTtA)
- [TSG95 Color Bar Generator Teardown](https://www.youtube.com/watch?v=gjlbBvNt404)
- [Moving from Codec to Camera, Tandberg teardown continued](https://www.youtube.com/watch?v=gQ5gPJepTi0)

## Misc 
- bitsquatting, rowhammer, aes encryption
- protocol analyzer tool, chip whisperer tool, shodan
- [Grokking Algorithms: An illustrated guide for programmers and other curious people](https://www.amazon.com/Grokking-Algorithms-illustrated-programmers-curious/dp/1617292230/ref=sr_1_2)
- [Lotte World](https://en.wikipedia.org/wiki/Lotte_World)
- haircuts!
- ice cream!
- feelings!

# THE END! 🎉  

There is no end! Never graduate!  

Thanks for reading!

~ ~ ~ 

# NGW'19

I did not take time off for this week, and I regretted it. I was able to spend some time in the space, see old friends, listen to lots of talks, participate in a few group discussions, including some deep dives into web archiving and digital preservation and video. 

# NGW'20 / two years later! What will I build?

This year, I took the week off and couldn't wait to see all of my friends spread over the globe, but then a global pandemic happened and everything has shifted into being remote-only. I am still taking the week off, and intend to focus on researching and building.

Like my time at RC, I will track some of my work here as a bit of a time capsule into what I explored during this time.

My research focus is on virtual worlds, past and present. I want to be able to structure my thinking around this topic in a way that is deeper than my own memory. I have a few other ideas, including visualizing and searching a PDF database, more adventures in digital divination, and focusing on CSS and SVG animations.

## Beginning of May

Trying to make up for long time? I have started planning what to work on and look into, which have shifted slightly from the paragraph above this one.

### Ideas
- techno-divination (continuing theme of aura-reader, i-ching, barthes-tarot, et al)
- visualization of archival material (have a collection of 3300 PDFs, how can I produce meaningful access?)
- network-based performance artwork
- exploring virtual worlds

### Code written
- [aura reader 2020](https://bits.ashleyblewer.com/aura-reader-2020)
- [jams page](https://ashleyblewer.com/jams.html) for me to track audio inspiration while in quarantine
- all the code and assets for a project that I have not yet checked into a git repo (rare for me!), more tbd. I usually don't hide things but this is something that is meant to be viewed in a specific way, and I don't usually do that, either.
- OCR and thumbnail generation for a set of PDFs, data transformation, small sqlite proof of concept also not quite ready for primetime

### Misc
- Her Majesty URL [video](https://vimeo.com/413896649), [etherpad](https://pad.profolia.org/URL#)
- [!!con 2020](https://bangbangcon.com) - absolutely all of it, it was a fantastic conference!
- [charli xcx demo ideas thread](https://twitter.com/FckyeahCharli/status/1248738826446610432)
- [Teenage Superstars](https://www.raindance.org/the-filmmaker-sessions/), the documentary
- [Spaceship Earth](https://neonrated.vhx.tv/checkout/screen-slate-presents-spaceship-earth/purchase), the documentary

## 2020-05-11 Monday

Here is where I will do a check-in of what I've done and what I plan to do yesterday and today. I think this is a useful way of keeping myself accountable even if it is similar to tactics deployed by power-hungry middle-managers seeking to control a workforce. 🙃

### Accomplishments
- configure DNS for network-based art project
- write artist statement
- reallife: [last class sendoff](https://github.com/ablwr/info654sp20/tree/master/syllabus)
- remembering to stretch neck/shoulders

### Misc
- State of RC
- the work of my students!!! wonderful but not share-able, sorry
- [emma rae norton - the mouse holds us](https://doodybrains.github.io/the-mouse-holds-us/)
- [You shouldn’t need to be a web historian to use web archives, Ian Milligan U Waterloo](https://www.youtube.com/watch?v=Ki-QGu9AGiQ)
- [Secrets of the Surface - official trailer](https://vimeo.com/380123288)
- [LIMA ONLINE: Joan Heemskerk (JODI) in conversation with Heath Bunting, moderated by Florian Cramer](https://www.youtube.com/watch?v=bNHJCkR39Kk)

## 2020-05-12 Tuesday

Today I remembered that doing things right takes time. Repetition and testing. Some things can't be rushed through. 

### Accomplishments
- still stretching
- html/css up an intro-site to give context, refine artist statement, and...
- [Throttled](https://ashleyblewer.com/throttled.html) is now live, sending it to testers before I can feel like it's really wrapped! Checking "network-based performance artwork" off the list -- I am really happy with this. It feels like there's not much to talk about technically, but maybe I will write a blog post about it since I did some diving into a few places I hadn't explored before.
- reallife: time to give students meaningful feedback on their final projects! this took a lot of time and talking about it in detail is not appropriate for these notes
- Finishing the ebook for Normal People before it gets auto-returned to the library in 24 hours

### Misc
- Checked out my [sibling in NGW note-taking!](https://github.com/saoirse-zee/rc-ngw-2020/blob/master/README.md)
- [AMRO2020 program](https://www.radical-openness.org/en/program/2020)
- breaktime: watching nontechnical talks! 
- [VirtuaVerse](https://store.steampowered.com/app/1019310/VirtuaVerse/), I want to play this game?

## 2020-05-13 Wednesday

Lots of social/group learning events today! Excited for: web standards disucssion, weird internet spaces, apl, intersectional feminist scifi talk, caaaats. 

I am trying to switch gears and into the meaningful archival access project, but still hanging on to finishing up Throttled with regards to blog-post writing and formalizing notes so I don't forget in the future.

### Accomplishments
- Took a break to [remove some jQuery](https://github.com/amiaopensource/ffmprovisr/pull/425)
- I have stretched, and I [am buying an expensive pillow highly recommended by a fellow RC'er](https://www.ecosa.com/pillow) to enforce good posture even when sleeping
- [Blog post](https://bits.ashleyblewer.com/blog/2020/05/13/throttled-a-few-things-i-learned-making-this-network-based-performance/) for holding Throttled notes. Maybe I'll give a talk about this on Friday?
- reallife: its grant-review season

### Misc
- [Curating Online Exhibitions Pt 1](https://rhizome.org/editorial/2020/may/13/curating-online-exhibitions-pt-1/)
- a bit more [likelike gallery touring](https://omoma.glitch.me/)

## 2020-05-14 Thursday

Yesterday was the halfway point, and I haven't gotten back into the archival access project, but hope to make a lot of progress on it today -- now that is my sole focus, now that the other project is out of my brain and in the world. This morning, I am going to start with writing what I've already done with the assumption that that will lead me to where I need to go in a way that feels more inviting than my todo list.

### Accomplishments
- Made a lot of progress on a forthcoming blog post about this week's project

### Misc
- reallife: it is still grant-review season, deadline imminent
- reallife: signed a contract for a small but impactful project :)
- I just keep [opening this](https://webassembly.org/docs/c-and-c++/) and eventually closing it 🤦
- ["The museum does not exist"](https://www.ssense.com/en-us/editorial/culture/the-museum-does-not-exist)
- Trader Joe's Organic Tusi Holy Basil Herbal Tea ☕
- Browsing [Open source, experimental, and tiny tools roundup](https://everest-pipkin.com/teaching/tools.html) and wishing I had more time!
- a friend and new coworker wrote something personal and I read it and cried because I'm so happy for her. 😭💖
- 04. Charli XCX - 7 years.mp3
- [This](https://stackoverflow.com/questions/7042340/error-cant-set-headers-after-they-are-sent-to-the-client) is a very thorough StackOverflow answer listing out Node/Express response methods, something I didn't easily find elsewhere.

## 2020-05-15 Friday

Last day :(

### Accomplishments
- lightning talk on Throttled
- lightning talk on the Vasulka archive project
- [blog post](https://bits.ashleyblewer.com/blog/2020/05/14/notes-on-exploring-the-vasulka-pdf-archive/) with notes about the Vasulka exploratory project. I want to spent two more days on this and then wrap it up completely, since I didn't get to spent the full week focused on it -- really only just a couple of days.

### Misc
- lots and lots of presentations
- [AI in the library, round one](https://andromedayelton.com/2020/05/15/ai-in-the-library-round-one/)
- [!!con recap post](https://thewebivore.com/con-2020-virtualbangbangcon/)
- [Artbase re-design](https://sites.rhizome.org/artbase-re-design/)
- [Unscroll: An Approach to Making New Things from Old Things](https://www.youtube.com/watch?v=BykYu4qA-bQ)

## 2020-05-16 Saturday

And that's a wrap! There's more I want to do, but I have to start acclimating back into reallife obligations.

NGW is such a refreshing burnout-prevention supplement. It's not the cure, but it helps get you there.

~ ~ ~ 

# NGW'21
**THREEEE years later! What will I maintain?**

Year three of Never Graduate Week and I'm focusing on not not shipping anything, doing maintenance work on existing things, and learning/practicing old skills.

A short list of things:
- Make color change consistent on the [I Ching](https://bits.ashleyblewer.com/i-ching/) (this is like a 5min fix, why do I procrastinate on it so much?)
- make and apply custom "sleeping" or "powered down" screens to my [reMarkable2](https://remarkable.com/store/remarkable-2)
- clean up old laptop
- set up new laptop
- thinking about trying a new Linux distro, which means I need to think about Linux distros
- so many code editor things annoy me and I just put up with it, I'd like to be more intentional about this arrangement
- improve thinking and structure on a long-form writing project
- some sort of [Exercism](https://exercism.io/) practice
- I got firefox tabs for days

# 2021-05-09 Sunday

- Made sure my equipment id set up and working for tomorrow's e-ink display workshop
- watered plants, planted some new seeds, repotted plants
- bought a new personal computer (a long-coveted Dell XPS 13"), feels good

# 2021-05-10 Monday

Something I have a really hard time learning is how to chill out and take a break, which has been very detrimental to my health. I'm trying to focus on that this week -- body/brain maintenance is part of the maintenance stack, after all.

### Accomplishments
- Signed up as a patreon for the [Tech Won't Save Us](https://www.patreon.com/techwontsaveus) podcast.
- gave myself a manicure with stick-on nail decals
- made three healthy little salads

## E-ink
- attended a very cool [e-ink workshop](https://github.com/m-clare/NGW_E_Ink_Workshop)
  - also needed to `apt-get update` and install pip3
  - `sudo apt-get install libopenjp2-7 libtiff5 libatlas-base-dev`
  - Enabling SPI via `sudo raspi-config` (here's a [how-to](https://www.raspberrypi-spy.co.uk/2014/08/enabling-the-spi-interface-on-the-raspberry-pi/))
  - this later broke, and I need to figure out why it doesn't think there are any more events today when there are
  - I also want to add images
  - Also the time is UTC and showing it in MYYY time would be good
  - [Here](https://twitter.com/ablwr/status/1392128547565850625) is what it looks like

## Memex Tech Demos
These are just loose notes
- Context: ["As We May Think"](https://en.wikipedia.org/wiki/As_We_May_Think)

  - People working with/in memex technology
  - "An ideal, not realizable" / people present wishes/fantasies onto this device / everyone implementing it gives a personal approach to the problem
  - First up, Andrew
	  - I know Andrew has a talk on a similar subject, [!!Con 2018: Talking to my past self (without introducing temporal paradoxes!) ](https://www.youtube.com/watch?v=FnFYs5BdI0E)
    - data importers, interface like "verb:travelled near:bondi beach duration:>10"
  	- Typical ETL structure, APIs/scrapers template as Extraction, transform, load into JSON API
  	- everything organized as a graph, use that to travel through different parts of the system.
  	- another example: "provider:goodreads, involved:(abouts:(climate))"
  	- like the memex, it shows relationships, when read, other related things, etc
  	- interesting question about consent to geotag and name people, and whether this qualifies as like a journal
  	- Roam Research
  	- thinking the original idea of the memex was more about this kind of thing (personal journal type analogy) rather than archiving stuff
  	- it's like 100s of GBs, designed to run local but happens to run on DigitalOcean
  	- writing about this is on [this blog post](https://hyfen.net/memex/)
  - Next up is Joe
  	- frictionless micrologging lil script
  - Next up is Nick
    - [ArchiveBox](https://archivebox.io/) demo (I'm already familiar so I didn't take detailed notes sorry!)
    - canonicalization layer
    - can pull from bookmarks, all the bookmarking systems, etc
    - working on this project helps ensure archive-ability for himself and others/clients/projects/etc
   - Next up is Shae
     - working on tracking papers, their DOI, authors, etc
     - code is here: [https://github.com/shapr/fermatslastmargin](https://github.com/shapr/fermatslastmargin)

## Elementary OS
Thinking of going with this OS when I get my new personal computer (ETA: Friday!!!)

- [Human Interface Guidelines](https://docs.elementary.io/hig/)
- [Changing power settings in Elementary OS](https://www.ryanprior.com/posts/changing-power-settings-in-elementary-os/)

## Misc
- Reminder about this channel: https://www.youtube.com/user/eaterbc
- [Building a raspi OS from scratch](https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/os/)
- Finished [Fake Accounts](https://www.penguinrandomhouse.com/books/667731/fake-accounts-by-lauren-oyler/) by Lauren Oyler

# 2021-05-11 Tuesday
- The [I Ching](https://bits.ashleyblewer.com/i-ching/)'s background should be smooth, This has bothered me for so long, yet it was like a 5-minute fix!

## Building collaborative virtual spaces discussion
  - a bit more on [RC Together](https://www.rctogether.com/)
  - [GatherTown](https://gather.town/)
  - [Workadventure](https://workadventu.re/)
  - omg [this app](https://mashable.com/article/color-chat-messaging-app/) where you communicate only in rectangles!
  - IBM paper about using SecondLife after the financial crisis -- [Synchronous Interaction Among Hundreds: An Evaluation of a Conference in an Avatar-based Virtual Environment](https://www.researchgate.net/publication/221515759_Synchronous_interaction_among_hundreds_An_evaluation_of_a_conference_in_an_avatar-based_virtual_environment)


## Cyberspace Show and Tell 
  - LIKELIKE Gallery (easy to fork) -- love this one
  - Workadventure -- so cute and cool, works really well!
  - visiting ascii town - managed to sign the guestbook
  - sprout.place !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
  - walky.space 

## Streaming MEDIA / WebRTC
- https://webrtcforthecurious.com/
- https://webrtchacks.com/webassembly-experiments/
- https://github.com/pion

## Internet Girlfriend Club
- [Volume 10](https://internetgirlfriend.club/volume10/0.html) is here!!! It's been "ready" for a while (as in, I had enough entries to build a new zine) but hadn't had the time and mental space to put it together. YAY!!

# 2021-05-12 Wednesday

Morning
- ate a cookie and a lavender latte because I am on vacation

## Programming in other languages
- Edith gives a talk about translating the official python documentation into French
  - organized a translation sprint
  - "great way to do dev tools onboard - you will be using git, but not in prod"
  - "you will learn about the language you are translating into, even if its your native language"
  - "(espaces insecables = non-breaking spaces in english)"

I asked about funding, because I want the A/VAA to be translated but I want to pay people to do it. This work was pro-bono though, but this is Edith's career also.

I also asked about the variations of a language, like that there are many different types of official Spanish. This context is French, so there's a specific official French to look towards, but caveats to that are that everything is default-masculine, and there are other situational problems.

Another question is about when to translate technical terms like "commit" or "branch". This seems to be project-based, so like many things, it depends.

Janice laments that American English always dominates, like in CSS: `color: black` instead of `colour: black`

- Talk from Paul on [Dark](https://darklang.com/) and supporting multiple languages here
- using multi-language for search even if the actual variable names are in English

"some of the biggest challenges aren't technical, they are cultural"

- Daniel talking about a few languages written in other languages
  - Ramsey Nasser: قلب -- https://nas.sr/%D9%82%D9%84%D8%A8/
  - Yorlang, Yoruba programming language -- https://anoniscoding.github.io/yorlang/
  - Jon Corbett, Cree#, PhD project -- https://esoteric.codes/blog/jon-corbett
  - [Cree language](https://en.wikipedia.org/wiki/Cree_language)
  - "instead of if/then, a stream splitting into two different channels"
  - speak to the interpreter, a raven character. storytelling language.
  - "not just keywords but cultural logic into the language as well"

## Memex Challenges

- "most things decay in the order of magnitude of a decade"
- interchange formats are key
- markdown is great
- not wanting to be locked into a company ecosystem, and able to bring/use your own tools
- how do I structure a trial period for moving to a new system?
- coaching people to use memex technology
- hierarchies, flat lists, different things work for different people. how long do you try out not just a software, but the rituals around notetaking?
- FUSE bridge, org-mode, tagging
- panic driven development
- user-defined tag relationships
- k-means clustering tags
- ontology - defining tag synonyms - programming and software and computer engineering 
- different definitions of ontology flying around lolol
- sorting/filtering
- your brain is very good at filtering and bubble up things you're looking for with context
- archive folder, move things into there
- memex failure: facebook in general
- collecting for the sake of collecting
- what is the goal of the memex?
	- increasing surface area
	- ability to share with others
- [Arc](https://apps.apple.com/ca/app/arc-app-location-activity/id1063151918 ) (app location activity tracking, offline only, private, secure, etc)
- "how to take smart notes"
- [tarsnap](https://www.tarsnap.com/)

It's so interesting to bounce from the "programming in different languages" directly into a call with a small archives that is looking for some help/guidance and then right into the Memex discussion. Being right in the middle of archives world and tech world, I have so many thoughts/feelings about this but not sure how to articulate them well, so I am not going to! I think my primary thoughts are around how the LIS/archives field are based around community knowledge, instutitional knowledge (and the conflation that an instution's knowledge is the same thing as community/culture, because I'm not trying to paint this as all positive) and the memex conversations here are all about personal knowledge systems, boutique and unique-to-you work (not fully, but the general purpose for convening is a celebration of the different ways people work towards the same general goal).

# Misc
- [Researching the Leadership Gap for Legacy Projects: Sumana Harihareswara](https://www.youtube.com/watch?v=RV19i8nXkTM)  
- lack of pipeline to recruit and grow contributors with leadership and management skills
- [Dave Rice at V International Seminar on Digital Preservation](https://www.youtube.com/watch?v=JhDgoBn7bQk)  
- [Neta Bomani - Dark Matter](http://netabomani.com/darkmatter/)
- [Video Compression Basics](https://rastergrid.com/blog/multimedia/2021/05/video-compression-basics/)
- [The Forgotten History of Home Video](https://www.youtube.com/watch?v=30Uc-JxJzYI)


Got a tip
- https://worldradiohistory.com/

# 2021-05-13 Thursday

## Morning
- Making coffee and reading [How the Personal Computer Broke the Human Body](https://www.vice.com/en/article/y3dda7/how-the-personal-computer-broke-the-human-body)
- Searching for suitable flash drives, which are scattered all over the house
- Making a Linux bootloader
- Began working through [Exercism](https://exercism.io/)'s TypeScript track

## Midday
- [MenderConf 2021](https://mendercon.com/schedule/) -- watched the afternoon talks

## World Radio History
Can I build on last year's Vasulka work to make this easy to search, retrieve, discover?

# 2021-05-14 Friday

## Morning/Lunch/Afternoon/Evening
- Finally finished [Detransition, Baby](https://www.penguinrandomhouse.com/books/621886/detransition-baby-by-torrey-peters/) last night!
- Taking care of something I can't talk about yet
- My [Halt and Catch Fire Syllabus](https://bits.ashleyblewer.com/halt-and-catch-fire-syllabus/) had some CSS that was failing to render properly in Chrome, and people seemed to really like it and think it was the intended aesthetic, which is cool, but I fixed it so that it looks the same in Chrome and Firefox.
- [A New Session](https://anewsession.com/), a telnet-based zine, is out now!!!!! I spent the lunchtime reading it.
- Looks cool: [Future of the Browser Unconference](https://futureofthebrowser.web.app/)
- watched some presentations that fried my brain
- I've been waiting to read this piece about [Andrew W.K.](https://www.stereogum.com/2015589/andrew-wk-steev-mike/columns/sounding-board/) for so many years
- started [this book](https://www.newline.co/fullstack-react-with-typescript) about React/TypeScript
- Listening: [Another Morning, Another Pillows](https://www.youtube.com/watch?v=a3eCVTbixrQ)
- more presentations!
  - visidata.org
  - IoT hacking smart devices
  - activating plushies with ML so kids can design their own toy gestures
  - [Brownian Motion](https://en.wikipedia.org/wiki/Brownian_motion)
  - Rachel's work/art: https://www.joyofrandomness.com/
- End of NGW party!
	- I made a rhubarb cake which I kept calling a pie, but was obviously not a pie. It involved making meringue which I haven't done since I was a kid, and I somehow managed to do it while keeping up with the conversations in the RC "Kitchen" room. Also if I had read the instructions before I started, I don't know if I would have had gone through with it, but it was too late by the time I got to the "separate the eggs and whip each in separate bowls" bit.

Overall, this year I went to a LOT of events (and there were so many to attend!), and didn't try to focus on doing much else, which worked really well! I wasn't able to get to work setting up a new personal computer because it hadn't arrived in time, but I did manage to think/learn/discover a lot of things and fix a few tiny things that had been annoying me for a long time. Also, I read two whole books that had nothing to do with programming.

Given that the entire world is burnt out and I am no exception to that, this was a great way to spend a week.

I spent the next two days not opening my computer at all! Until next year!

~ ~ ~ 

# NGW'22 !!!

I think I'll be using this week to get a bunch of things that have been rattling around in my head OUT of my head. I like treating this week as a mini RC retreat, where I can give myself that extra permissions to think and explore and grow, completely unconstrained. 

Had plans to visit NYC and see friends, but cases are rising and I'm tired and Rory and I decided to stay home in Philly.

I have a LOT of things I want to work on, and not enough time for all of them!

- Pair with Rory on multi-platform music player
- Finish [aura-reader-for-two](https://github.com/ablwr/aura-reader-for-two), write about it
- I'm accidentally [making a book](https://twitter.com/ablwr/status/1514651214167826440) so I have a lot of goals around that, although I don't know if I'll necessarily be addressing them this week
- library reference room demo idea
- I wrote something down that says "VLC blog" and I have NO idea what that means? I'm not even sure the word is VLC? VCC?
- Finish co-authored blog post about Archive81
- Paint bedroom walls; finish painting back patio
- something something gstreamer...

## 7-8 May (Sat/Sun)
Read (future tense and then past tense):
- [Glitch Feminism](https://www.penguinrandomhouse.com/books/646946/glitch-feminism-by-legacy-russell/), Legacy Russell
- [People I've Met From the Internet](https://www.spdbooks.org/Products/9781938900259/people-ive-met-from-the-internet.aspx), Stephen Van Dyck

## 9 May (Mon)

### Waking up

- [This tweet I made last night](https://twitter.com/ablwr/status/1523471448219602944) on what format you would pick to do longish-form writing on has me introspecting a lot more than I thought!
- [Kendrick Lamar - The Heart Part 5](https://www.youtube.com/watch?v=uAPUkgeiFVY)
- almond flour chocolate chip pancakes for breakfast
- [Five Koans of Software Architecture](https://bellmar.medium.com/five-koans-of-software-architecture-f9f7305598c2), Marianne Bellotti

### Afternoon
- New blog post: [I accidentally started making a book](https://bits.ashleyblewer.com/blog/2022/05/09/accidentally-making-a-book-video-format-illustrations/)
- briefly listen to a talk about Plan 9
- starting to read these [placement diaries](https://rozinaaamir.com/placement.html)
- [BandcampFS](https://medium.com/@__Tux/using-bandcamp-as-a-backup-solution-3b6549d24579) ???
- catch up with Julia & talk about printing opts
- TODO: catch up with Jean
- see Hannah I R L
- "small art talks" session, yay!!
- drafting some future blog posts to get book-related things out of my brain
