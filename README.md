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

## This will also be a living syllabus, 
updated with links to blog posts, works I produced, and things I used to tackle these problems or build things for each week.

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

# Week 1 (April 2-6) Containers/codecs

- Video container/codec review, how do significant properties relate to each other when established by each format?
- containers versus codecs, how do they work together (or not together?)
- Exploring Matroska attachments and file format polyglot-ing 
- (put mkv file inside mkv file)
- Understand how codecs are made 

# Week 2 (April 9-13)

- Begin manipulation of raw video data 
- Muxing, demuxing, compiling code  
- ffmpeg filters
- Visualizing compression: Is there a way to extract only-the-compression from audio or video for visualization purposes? 
- Build something in C 

# Week 3 (April 16-20)

- Colorspaces
- Subtitles 
- Codec manipulation

# Week 4 (April 23-27)

- Web Assembly, put C in the browser 
- Electron, put JS on the desktop

# Week 5 (April 30 - May 4)

- Thinking about open source contributions here

# Week 6 (May 7-11)

- Codec-building! rough drafts

# BONUS WEEK (May 14-18)

[!!Con May 12-13](http://bangbangcon.com/)

I thiiiiiink this is when Never Graduate Week happens. SPRING BREAKKKKKKKK

# Week 7 (May 21-25)

- Codec-building, codec-built 

# Week 8 (May 28 - June 1)

- Codec-building, codec-built 

# Week 9 (June 4-8)

- Steps to build a video player?

# Week 10 (June 11-15)

[ TBD: Intentionally unstructured play ]

# Week 11 (June 18-22)

[ TBD: Intentionally unstructured play ]

# Week 12 (June 25-28)

[ TBD: Intentionally unstructured play ]

# THE END!  

There is no end!

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