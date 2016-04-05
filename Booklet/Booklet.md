# Contents

# Introduction

Your guides:

* Martin Paulo
* Jared Winton

Some history:
ResBaz:
ResOS: a conceit

-- *Slide* --

# Software Carpentry: an overview

**NB** The ResOS training is *not* a Software Carpentry course. However, we have based the way the material
was developed and its content on many of the concepts and ideas that Software Carpentry taught us.

-- *Slide End* --

## History

So in order to understand the material, you should know a bit about Software Carpentry.

Software carpentry grew from the realization that researchers need to install and maintain software:
not only that - they need to occasionally write, debug and test it as well. Yet most researchers have
never been taught to do this!

A course to tackle this problem was developed and run by Greg Wilson and Brent Gorda in 1998.

From the delivery of this course they learnt that:

* Week long courses frazzle the attendees brains
* Textbook software development is not useful to researchers

Subsequent to this the course materials were put on line. Other iterations followed.

During this period it was realized that:

* Most computer scientists don't have an interest in solving this problem
* The target market are people in the first few years of graduate school

MOOC style courses were also attempted. From this came the realization:

* Video's are a huge amount of effort
* Most people don't complete the courses

After years of effort, review, and development, Software Carpentry now has the following format:

* A two day workshop
* Covering a small set of tools
* That introduce high level concepts
* With the goal of teaching computational competence

The following guidelines are in place

* No more than 40 people in a workshop
* If possible, parallel sessions, with attendees streamed by ability

If parallel sessions are run, then:

* A pre-assesment questionnaire is used to create the groups
* People are not swapped from group to group

The workshops aim to have:

* An instructor up front
* At least 1 helper per 8 attendees

Group sign up leads to better workshops and better attendance by under represented groups

## The following feedback loops are used:

Sticky notes are handed out to learners:

* two different colours (typically, Red and Green)
* used for true/false answers
* to show pain if not not coping
* and to signal that activies are completed

Minute cards:

Before each break the learners are asked to write one thing:

* that they've learnt on their green sticky note
* that they found confusing on their red sticky note

The instructor then collates these and incorporates the feedback into the next iteration.

Summary feedback at the end of the day:

Every attendee is asked to stand and to give one good point about the day, and one negative point,
without repeating what has already been said. The instructor makes notes and incorporates the
feedback into the next iteration.

Post workshop assessments:

After the workshop an assessment is sent to the attendees. These don't have high return rates.
Instructors are also requested to provide feedback in debriefing sessions.

## Delivery

* Live coding
* Two devices for the instructor
* An Etherpad session
* Learners work on their own machines
* Pair programming (so dinner table style rooms over lecture theaters)

## Biggest challenges

* Are they helping researchers?
* Diversity of learners - 20% bored, 20% lost :(
* People don't contribute back...

## So

Software carpentry has been under continuous iterative development for many years now. Along the
way the material has been reworked to take into account the latest in educational research and
feedback from the actual delivery.

BTW, Software Carpentry material is licenced under a creative commons logo. Anyone is free to use it.

**NB** But you are not free to use their name and logo! There are strict conditions applied to this. They
want to maintain their good name and reputation!

We thoroughly recommend that if you haven't you sign up for their trainers course!

# Myths and truths about learning and education

Software Carpentry have mailing lists. And some of the discussions and books that are pointed to are
very interesting.

So lets get our sticky notes out and practice with some fun things we've learnt from the mailing lists.

-- *Slide* --

## People have different learning styles

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** False - it's true that we have preferred learning styles. But our preferred learning style
is probably not be our best learning style...

Further, learning styles are typically given a granular nature and labelled ("Visual!", "Auditory"), but us humans
actually form a continuum. Preparing lessons for a label short changes the continuum.

-- *Slide* --

## Physical activity helps learning

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** True - Activity makes for a healthy brain. Especially true for children!

-- *Slide* --

## Google makes learning obsolete!

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** False - Would you let a brain surgeon near you who going to Google every step of your operation along the way?
I wouldn't.

We need context and a mental structure to make sense of the facts we find on the Internet. Context and structure
we get from learning... In fact, given the amount of information available on the Internet we might need more
learning to make sense of it all!

-- *Slide* --

## Knowledge: as perishable as a fresh fish!

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** False - Is the knowledge that you have, somehow, in some strange quantum way, flipping from correct to wrong?
Or is it simply that the knowledge available is exploding? Sure, some of the knowledge we may hold dear may turn out
to be incorrect (Carbs are good for you?), but the majority still holds true. Pythagoras Rulez!

-- *Slide* --

## Discovery trumps explanation

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** True and False - Both sides have a point. If you can learn quantum physics by discovery: well, why are you
in this room? Research has shown that pure discovery learning doesn't work: but guided investigative learning can be
very effective in certain settings.

-- *Slide* --

## Memory records exactly what we experience...

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** False - Sadly it's been proved that not only is our memory of what we experience highly unreliable, it's even
posssible to plant false remembered experiences through clever questions.

-- *Slide* --

## BTW: who'se seen this:

<iframe width="420" height="315" src="https://www.youtube.com/embed/vJG698U2Mvo" frameborder="0" allowfullscreen></iframe>

-- *Slide End* --





# How learning works


# Personas: an introduction

Now, I want you to break up into groups of 3-4 people.

The first exercise that I want you to do as a group is to develop a persona for your group.

"What's a persona?" I think I hear you ask.

A persona is the representation of the goals and behaviour of a group of hypothetical users.

The theory is that by understanding the needs and abilities of that persona, you can better satisfy the needs and
abilities of the larger group.

A good persona should represent a skill set and a behaviour pattern - not a job description.

By example, here's a persona that I developed:

## An Astronomer at a University

**Name:**     Associate Professor Glenn Bording
**Job title:**     Senior researcher and lecturer, Radio Astronomy group

**Demographics:**

* 40 years old
* Programming experience in C and Fortran
* Basic HPC experience
* Prefers to work with physical hardware

**Background:**

* While preparing a new course for undergraduates, developed a computing challenge to support research using real data
* Realised the BYOD for most students were not powerful enough
* Labs not suitable for task
* Teaching parallel programming and getting accounts for students would be difficult
* Heard about the research cloud

**Goal:**

* Now keen to learn about ResOS to see if it solves this problem.

Once you, as a group, have agreed on your persona, hold up a green sticky note. But you'd better be quick, because
I'm giving you only 5 minutes!

Ok: for our purposes today, the persona's that you have developed represent the people that you will be explaining
our ResOS training course to.

So as we go through today I want each group to ask themselves just what it would take to communicate the concepts or
activities we are covering to this persona.

If you find you can't do it, then stop me, and we will all discuss it and see if we can come up with a better approach.
*Ask for one or two persona's to be read out*

# How to access the course material

# A walk through the course material

# Preparation for the day

Find out about the venue. Does it have enough:

* Seats
* Tables
* Power points
* Network connectivity


* If you are going to stream people, send out a pre-assessment questionnaire
* Enough sticky notes, in two different colours, to hand out to attendees at the start
  and after each break



# A discussion on delivering the course material

# Course feedback

# How to contribute changes back to the course
