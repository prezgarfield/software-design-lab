# Rob's Technical Journal

dropbox link: https://www.dropbox.com/sh/qgyrt3325y606sf/AADK4REvuFROf-u1YzZ4jeWla?dl=0

## Week Two (1/30 to 2/6)

So far this week, I got Git Bash up and running on my home desktop and created this repository from the command line.  I copied over, using cmd line still, the templates from Patrick's repo for the class.  I also created a new Python project which pulls in a set of sentences from a csv file, rearranges them with a shuffling algorithm, then creates a new MS Word document (python-docx) and prints the shuffled set of sentences punctuated by stochastically generated chapter and paragraph breaks.

Started learning the Spacy library for Python. Was able to install the library and a grammar using pip then tried to feed all of the aforementioned sentences into the grammar for parsing.  Since there are about 10k sentences, I hit a memory cap, so I rewrote the parsing function to take smaller chunks of text in at a time.  That worked.  Now, what to do with them?

I created a db using SQLite and could probably use a little help figuring out how best to configure it.  I'd like to keep sentences, tags and tree parses in each record, but I'm not sure exactly where this is going so it is hard to come up with a good model.

Tomorrow, I'm hoping to make Jonathan Reeve's word embedding workshop at the xpMethods lab.  More then.

Note to self: Always start off the day's gitting with a status and a pull.  Always end with a status and, perhaps, a push.


