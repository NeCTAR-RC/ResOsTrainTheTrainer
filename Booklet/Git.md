# Git - and our lessons

As you have seen, the course material is kept under version control.

-- *Slide* --

### Do you know what git is?

* <span style="color:green">&#9632;</span> = Yes.
* <span style="color:red">&#9632;</span> = No.

-- *Slide End* --

**NB** If there are any "No's" you have to explain git...

The following may help you:

* https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
* https://git-scm.com/book/en/v2/Getting-Started-Git-Basics
* http://tom.preston-werner.com/2009/05/19/the-git-parable.html
* https://matthew-brett.github.io/pydagogue/curious_git.html

-- *Slide* --

### Which of these is false:

Git:

1. Is a version control system
1. Is a distributed version control system
1. Is able to run offline
1. Has three states for files: modified, staged, committed
1. Can do your head in...

-- *Slide End* --

Discuss each of these options further before asking for the answer.
For Option E you can use this:

"*Git has a very simple and powerful underlying model. Atop this model is piled an immense trashheap of confusing,
overlapping, inconsistent commands. If you try to just learn what commands to run in what order, your life will be
miserable, because none of the commands make sense. Learning the underlying model has a much better payoff because
it is much easier to understand what is really going on underneath than to try to infer it, Sherlock-Holmes style,
from the top.*" - [Mark Dominus](http://blog.plover.com/prog/two-things-about-git.html)

**Answer** I believe them all to be true...

Any confusion here should require further discussion...

Not only is the course material kept under version control: that version control is accessible via an online
repository, so you can revisit it at any time, use it as a stand alone course if you want to, and even, hopefully,
contributes changes and extensions back!

To check the course out onto our local machine we do the following:

```bash
git clone https://github.com/resbaz/nectar-cloud-lessons.git
```

**Question** Can you check the lessons out?

Hold up a green card when you are done
And a red card if you need help.

The exciting thing about our repository is that we actually include a reference to another repository.

So to get a copy of the child repository we need to tell git to update the local configuration files
with information about any referenced repositories.

```bash
git submodule init
```

**Question** Can you init your submodules?

Hold up a green card when you are done
And a red card if you need help.

Once we've done that we tell git to fetch any referenced repositories.

```bash
git submodule update
```

**Question** Can you update your submodules?

Hold up a green card when you are done
And a red card if you need help.

What is this referenced repository, I hear you ask?

Well, to quote someone

-- *Slide* --

"I've got a plan so cunning, you could put a tail on it and call it a weasel<sup><small>1</small></sup>"

AKA: [REVEAL.JS](http://lab.hakim.se/reveal-js/#/)

<small>1: [Blackadder](https://en.wikiquote.org/wiki/Blackadder)</small>

-- *Slide End* --

Reveal.js is a Javascript presentation framework. It's really cool

We have written a tool that that chunders through our lecture notes...

-- *Slide* --

### SlideExtractor.jar

`-- *Slide* --`

In the lessons any text between lines that have only the above marker

And finish with only the below marker

`-- *Slide End* --`

Will extracted into a lesson slide.

-- *Slide End* --

Demonstrate on the command line

```bash
ls  # show the jar and the properties file
java -jar SlideExtractor.jar # need to have Java. Talk about language choices  And VM choices!
open ./Presentation/Lesson_I.html  # show in browser
```

The reason for doing this was because it means that our slides and lecture notes all live in the same file.
Hence:

* As we are working through them we can see what will be coming up next.
* We don't have to maintain separate presentation material.
* It should help people who use screen readers track what's happening.

Also we/I am toying with the idea of splitting out the questions into a separate file: and of writing an app
to allow us to get users to actually select these from within a browser window. So that we can gather metrics
about the responses.

-- *Slide* --

### Discuss!

Are clickers a good idea?

-- *Slide End* --

The downside of our slide extractor is that we run the risk of sinking into the [PowerPoint trap](http://users.ha.uth.gr/tgd/pt0501/09/Tufte.pdf)

We've divided the material into one file per lesson.

And there's no need for you to generate the slides: we've checked the generated slides into the repository.

-- *Slide* --

### To give the lessons (basic)

1. [ ] Clone the repository
1. [ ] Update the repository submodules
1. [ ] **Optional:** Checkout the tag you want to deliver
1. [ ] **Optional:** Update the introductory slide with your name
1. [ ] **Optional:** Regenerate the slides
1. [ ] Open the lesson slides in your browser!

-- *Slide End* --

BTW, I just print the lesson plans off of GitHub: which does a beautiful job of rendering the
markdown.

-- *Slide* --

### Can you open, say Lesson_II.html in your browser?

And step through some of the slides?

* <span style="color:green">&#9632;</span> = Yes.
* <span style="color:red">&#9632;</span> = Houston, we've had a problem here!

-- *Slide End* --

We've settled on the following way of managing the material:

There is a version number at the top of the README.md.
That version number corresponds to the last tagged copy.
If we are going to deliver the course and there are lots of changes since the tagged copy given by the
version number, we create a new version and tag it.

This means that you should always be able to go back to a particular version in time.

-- *Slide* --

### What's the current version number?

1. 1.0.0
1. 1.0.1
1. 1.1.0
1. 1.1.1
1. 1.2.0

-- *Slide End* --

To fetch all the tags from the remote origin:


```bash
git pull --tags
```

Then to see a list of the tags

```bash
git tag
```

-- *Slide* --

### Can you list the tags?

* <span style="color:green">&#9632;</span> = Yes.
* <span style="color:red">&#9632;</span> = No.

-- *Slide End* --

GitHub shows you, but if you want see the commits between the last tag and now locally

```bash
git log --pretty=oneline master...1.0.0
```

You might have to explain the above command on a board...

-- *Slide* --

### Are there are any commits since the last tag?

* <span style="color:green">&#9632;</span> = Yes.
* <span style="color:red">&#9632;</span> = No.

-- *Slide End* --

It's good to check to see if there are any changes since the last tag: and if you want to include them
in your lessons or not.

If you have a set of notes for a particular version of the course, and that's what you want to
deliver you can checkout that particular tag and use it.


How to checkout a specific tag as a local branch:

```bash
$ git checkout tags/<tag_name> -b <tag_name>
```

-- *Slide* --

## Can you checkout version 1.0.0?

* <span style="color:green">&#9632;</span> = Yes.
* <span style="color:red">&#9632;</span> = No.

-- *Slide End* --

-- *Slide* --

### True or False: Google makes learning obsolete!

* <span style="color:green">&#9632;</span> = True.
* <span style="color:red">&#9632;</span> = False.

-- *Slide End* --

**A** False - Would you let a brain surgeon near you who going to Google every step of your operation along the way?
I wouldn't...

We need context and a mental structure to make sense of the facts we find on the Internet. Context and structure
we get from learning... In fact, given the amount of information available on the Internet we might need more
learning to make sense of it all!


