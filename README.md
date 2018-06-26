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

## AV1
- [AOM AV1 codec mapping in Matroska/WebM draft](https://github.com/Matroska-Org/matroska-specification/blob/av1-mappin/codec/av1.md)
- [av1 1.0.0](https://aomedia.googlesource.com/aom/+/v1.0.0)


## Misc 
- bitsquatting, rowhammer, aes encryption
- protocol analyzer tool, chip whisperer tool, shodan

# THE END! 🎉  

There is no end! Never graduate!

# Mini-projects

Some ideas I have for small projects to work on!

## Birthday planet map generator -- hey I did this!
 
Generate an image that shows the state of the solar system at the time of someone's birth and text that explains how that aligns to someone's astrological sign (and moon sign, and rising sign). I think this mini-project will involve: Understanding the rules of astrology, some math about how fast planets move around the sun in relation to each other, ImageMagick to produce a proper image.

## Significant contribution(s) to Audiorecorder

[Audiorecorder](https://github.com/amiaopensource/audiorecorder) is a small, simple audio digitization command-line tool that has recently pushed up a new GUI made in Shoes (Ruby). It can use some help in making the application run a little bit better using this new framework.

## Recreating computer/video art in CSS or Processing.js

Learn how to better use Processing, new CSS features, or new HTML5 features by recreating early computer/video artworks. lillian schwartz, vera molnar, ken knowlton, john whitney, manfred mohr, dara birnbaum, paul sharits, hollis frampton, michael snow, nam june paik, stan vanderbeek are all potential artists to be inspired by and whose work I can attempt to replicate. I think this may involve some math.

## Linter?

Write a linter? A few starting links:
https://stackoverflow.com/questions/70705/how-to-write-a-linter  
https://github.com/mcandre/linters  
