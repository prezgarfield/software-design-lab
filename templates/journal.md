# Rob's Technical Journal

dropbox link: https://www.dropbox.com/sh/qgyrt3325y606sf/AADK4REvuFROf-u1YzZ4jeWla?dl=0

## Week Two (1/30 to 2/6)

So far this week, I got Git Bash up and running on my home desktop and created this repository from the command line.  I copied over, using cmd line still, the templates from Patrick's repo for the class.  I also created a new Python project which pulls in a set of sentences from a csv file, rearranges them with a shuffling algorithm, then creates a new MS Word document (python-docx) and prints the shuffled set of sentences punctuated by stochastically generated chapter and paragraph breaks.

Started learning the Spacy library for Python. Was able to install the library and a grammar using pip then tried to feed all of the aforementioned sentences into the grammar for parsing.  Since there are about 10k sentences, I hit a memory cap, so I rewrote the parsing function to take smaller chunks of text in at a time.  That worked.  Now, what to do with them?

I created a db using SQLite and could probably use a little help figuring out how best to configure it.  I'd like to keep sentences, tags and tree parses in each record, but I'm not sure exactly where this is going so it is hard to come up with a good model.

Tomorrow, I'm hoping to make Jonathan Reeve's word embedding workshop at the xpMethods lab.  More then. [note: did not make it.  Spoke to Jonathan a bit last Friday about getting up and running on my own.]

Note to self: Always start off the day's gitting with a status and a pull.  Always end with a status and, perhaps, a push.

## Week Three (2/7 to 2/13)

Coding:
Spent over 8 hours developing a python program that takes in a video file (works so far with mp4 and avi, using cv2 (so probably other formats as well), breaks it into frames, stores the frames, runs rbg averaging and rbg medianing(sic?) algorithms to produce 2 new images.  Popped some of these up in an Instagram account.  Instagram sucks for high res stuff, though, so I'll move them somewhere else where they can be viewed full size.  I haven't yet set up the avg/median algorithms to avoid memory issues, so I'll do that today.  Sequence: 1) Just run (hardcoded)X number of frames at a time, clear memory between, then avg/med composite images then 2)check available memory to determine total available and dynamically determine X from the frame size.

Reading:
Read back over the Learning Python the Hard Way exercises.  I'm comfortable with all it is asking us to do.  Some of the commands (like "print") presuppose an earlier Python version.  The Dear Developer article is fun and concise.  I like the argument that accessibility should be a fundamental front end web development skill.

## Week Four (2/14 to 2/20)

Coding: 
Spent about 3 hours looking into the TEI guidelines and am wondering if anyone has done any programmatic work towards automating TEI encoding of text.  Read over some TEI parsing examples from Github.

Spent about an hour getting Spacy and Word2Vec added to a venv in my Anaconda install.  Patrick, you are right about PyCharm.  It's pretty awesome!

Refined a bit of the video averaging program to handle files and directories better.  Fixed a directory bug.  Still haven't fixed the issue with memory problems which is holding me back from processing large amounts of image files.  Got sick on Monday and haven't been as productive as I'd like; usually, I have Mondays and Wednesdays to focus on this class.
