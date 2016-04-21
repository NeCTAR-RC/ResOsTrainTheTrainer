# Readme

This a the material for a "Train the Trainers" event. 

The trainers are preparing to deliver the [NeCTAR cloud lessons](https://github.com/resbaz/nectar-cloud-lessons).

It is assumed that the trainers recieving this training

## Git

If you check this repository out be aware that it uses Git submodules to manage the reveal.js dependency.
To also clone reveal.js, you will have to either:

    # fetch it all in one hit
    git clone --recursive https://github.com/MartinPaulo/ResOsTrainTheTrainer.git

Or:

    # take it step by step
    git clone https://github.com/MartinPaulo/ResOsTrainTheTrainer.git
    git submodule init
    git submodule update

## To regenerate the slides

The SlideExtractor.jar in the root directory will re-create the slides if needed.

To run it ensure that the java version installed is java 8:

```bash
java -version
```

should return something along the lines of `java version "1.8.0_65"`.

If it doesn't then install java 8 from here: http://www.oracle.com/technetwork/java/javase/overview/java8-2100321.html

Then in a command prompt in the root directory simply issue:

```bash
java -jar SlideExtractor.jar
```

You should see something like the following fly by:

```bash
Working on: ./Booklet/Booklet.md
Writing to: ./Presentation/Booklet.html
Writing to: ./Presentation/index.html

```

# Attendees prerequisites for this course

1. [ ] A [GitHub account](https://github.com/join)
1. [ ] Git locally installed
1. [ ] An active account on the NeCTAR dashboard

# Instructor's notes

Check that the [etherpad](https://etherpad.wikimedia.org/p/ResOsTtT) exists. If not, recreate it using the
downloaded [version](Etherpad/ResOsTtT.etherpad)
Remember to always walk through your slides when you regenerate them!

# Preparation for delivering the actual course.

To give the lessons, you need to

1. Clone the repository
1. Update the repository submodules
1. **Optional:** Checkout the tag you want to deliver
1. **Optional:** Update the introductory slide with your name
1. **Optional:** Regenerate the slides
1. Open the lesson slides in your browser!

So, you, the presenter, will need to:

1. [ ] Have an AAF account
1. [ ] Have checked the training material out of GitHub
1. [ ] Have a terminal of some kind that you can ssh into instances with

We suggest getting attendees to log onto the NeCTAR cloud, and to install any needed software
before the day.

So before the day, send out an email message to attendees advising them of the 
[prerequisites](https://github.com/resbaz/nectar-cloud-lessons/tree/master/Prerequisites).

Find out about the venue. Does it have enough:

1. [ ] Seats
1. [ ] Tables
1. [ ] Power points

Does the venue have:

1. [ ] Network connectivity (wifi)
1. [ ] Internet access
1. [ ] A big display you can use
1. [ ] A whiteboard (or paper) that you can draw on
1. [ ] Pens (and cleaner for the whiteboard)

What kind of connectors do you need to bring along for your devices?

Do you have:

1. [ ] Network connectivity (eg: are you banking on having EduRoam work for you, and have you tested that it is available
  and does indeed work for you...)
1. [ ] Enough sticky notes, in two different colours, to hand out to attendees at the start
  and after each break
1. [ ] A set of answer cards, enough for each learner, lettered 'A', 'B', 'C', 'D' and 'E' respectively.
1. [ ] A set of three envelopes, at least one of which fits inside the other two, to describe ssh and man in the middle
  attacks.
1. [ ] Any other props you might like to use?
1. [ ] A set of spare pens for people to write on the sticky notes with (It would appear in this digital age a
  lot of people travel penless)?

The image to be used:

1. [ ] Is the image named `res_os_drupal7` available and public on the NeCTAR cloud?
1. [ ] If so, check that it works as expected. Make a snapshot so that you have a fall back image.
1. [ ] If it's not there, or doesn't work as expected, make a new image to use.

Have you checked the slides are all as you expect?

On the day:

1. [ ] Each learner will need a laptop with wifi access
1. [ ] Do you need to deal with Chromebooks? Crosh Or Chrome Shell might be needed
1. [ ] Each learner on the course must have an AAF logon.
1. [ ] Each learner must have an allocation on the Research Cloud that they can use.


On the day for those that have expired trial projects you can:

1. [ ] get them to pair up with others
1. [ ] have a special tenancy for the lesson, and then add them to it on the fly.
  This may not a great solution as people in the tenancy will step on each others toes. But is has worked for us.
1. [ ] have someone on hand to extend their trial tenancies on the spot?

If you are going to stream people, devise and send out a pre-assessment questionnaire. We'd love a copy!

## Afterwards...

* Collate the feedback. Is any of it actionable?
* Remove users from a shared tenancy (if you had to add any)

# Some links

* The software carpentry store: http://www.cafepress.com/swcarpentry
* Log shell output to Etherpad: https://github.com/c-martinez/shellther
* http://sciencecases.lib.buffalo.edu/cs/pdfs/Clicker%20Cases-XXXVI-2.pdf


# To Resolve

1. [ ] As in Software Carpentry, should trainers who submit a GitHub correction get a certificate?
1. [ ] What about a code of conduct: http://software-carpentry.org/conduct/
1. [ ] Add a backing etherpad
1. [ ] Send out reminder email about the post day survey...