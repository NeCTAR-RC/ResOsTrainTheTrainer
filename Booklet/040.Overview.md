# An overview of the course material

-- *Slide* --

### The material can be found at:

* https://github.com/resbaz/nectar-cloud-lessons

Can you open this in your browser?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

## How we developed the course.

* We did a concept map on paper.
* Then we created a template for each lesson plan.
* We used the lesson plan to develop each lesson.
* We gave trial deliveries of each lesson to guinea pigs.
* We modified the lessons to match what we learnt from the trial delivery.

The lesson plans are in the repository, under the "Planning" folder. They give a high level overview of each of the
lessons.

-- *Slide* --

### Do you think we have kept the lesson plans up to date?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

**Answer:** We have tried. But like so much documentation in the software world, we struggle :(

But in getting to grips with a lesson, reading the lesson plan and ensuring that you understand the concepts
the lesson is attempting to convey is key.

-- *Slide* --

### Can you find and open the lesson plans?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

Follow along in the lesson plan as we discuss the lessons.

## Lesson 1

We do a high level drive through of the dashboard: and keep the learners engaged by playing a game of follow my
leader: and by asking questions as we go. In the end the instructor launches an instance: but it's not intended
for the class to follow suite...

-- *Slide* --

### What's an ephemeral disk?

1. A quantum disk
1. A disk that moves from VM to VM
1. A disk that only exists for the life of its VM
1. A made up word set
1. Something victorians put their tea cups on

-- *Slide End* --

**Answer:** C. A disk that lives only for the lifetime of its associated VM.

-- *Slide* --

### What's a NeCTAR image?

1. A picture at an exhibition
1. A representation of NeCTAR
1. The general impression that NeCTAR presents to the world
1. A file that contains the contents of a hard drive
1. A fine piece in the NeCTAR art collection

-- *Slide End* --

**Answer:** D. A file that contains the contents of a hard drive.

-- *Slide* --

### No one really does anything in this lesson!

Is that a problem?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

Discuss that we've tried mixing lesson 1 and two up: and that we've had best success by introducing the concepts
and then the hands on work.

## Lesson 2

We get the students to create their own security group, keypair and then launch their own instance.

We scaffold this by giving them checklists to follow.

-- *Slide* --

### Jared's lesson

Don't print out the checklists!

-- *Slide End* --

BTW: this is how we communicate key pairs (give a run through of Pem the greek merchant banker...)

-- *Slide* --

### Our keypair analogy

Is it a problem?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

If it's a problem, we'd like to have a better one!

## Lesson 3

Our most ambitious lesson so far!

We introduce the command line, ssh, sudo, package management and show security groups in action.

### A secret...

The command line is in here because of our historic baggage.

Outside of our focus groups, we've never done the command line play and the command line itself.

This is because of where and when these lessons have been given.

I want to move it out into its own lesson.

-- *Slide* --

### Discuss!

What to do with the command line?

-- *Slide End* --

-- *Slide* --

### Our biggest problem...

The amazing teleporting terminal!

-- *Slide End* --

Hence our increasingly laboured explanations around terminals...

-- *Slide* --

### Our ssh analogy

Is it a problem?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

Can anyone think of a better one?

-- *Slide* --

### Our eve in the middle analogy

Is it a problem?

* <span style="color:white;background:green">G</span> = Yes.
* <span style="color:white;background:red">R</span> = No.

-- *Slide End* --

We are finding it more fun to do a play with one of the helpers playing out the roll of the eavesdropper in the middle:
and no envelopes!

Also, we put this in because when we first started delivering this course the NeCTAR scheduler was aggressively
reusing IP numbers and users would run into this issue often. Now that Neutron is in the mix this no longer the case.
Perhaps we could dress down the warning?

## Lesson 4

We get our learners to use scp and CyberDuck to move data to and from their remote machines.

-- *Slide* --

### Moving data: our top researcher request!

Hence it's worth spending time on...

-- *Slide End* --

## Lesson 5

We launch and run graphical applications via XWindows over ssh.

-- *Slide* --

### Graphical applications: our top promoter request!

Of interest...

-- *Slide End* --

-- *Slide* --

### X-Windows

Where's the XServer?

1. On the users workstation
1. On the remote VM
1. Does it matter?

-- *Slide End* --

**Answer:** A, in our case. We don't really dive into this, just because of the amount of confusion
it can engender.

## Lesson 6

We dive deeper into snapshots and scaling.

-- *Slide* --

### Why are NeCTAR snapshots broken?

1. They are just too easy to do: suspicious enough!
1. The magic nostrums aren't up to the task!
1. They are not broken! How dare you!
1. The state of the machine is not captured
1. Cosmic rays can flip their bits.

-- *Slide End* --

**Answer:** D. Whilst E is a topic for a good debate, the answer is: D. The state of the machine is not captured

This seems to be a little known fact :(

We teach a work around that gives faultless snapshots.

-- *Slide* --

### Anyone care to guess our technique?

-- *Slide End* --

**Answer:** Yes, we shut the VM down. Note: Not terminate!!

-- *Slide* --

### Do you know the differences between:

1. A soft reboot of a VM
1. A terminated VM
1. A paused VM
1. A stopped VM
1. A hard reboot of a VM

###?

-- *Slide End* --

A paused VM is simply halted in memory, ready to be started again.
A stopped VM has its state written to the host machines disk, ready to be resumed from there.
A soft reboot tries to do a graceful reboot (you ask the OS to reboot).
A hard reboot just reboots the machine! (you press the button)

## Lesson 7

We have a very clumsy display that transient storage is not to be relied on.

And also do some vertical scaling and public sharing of snapshots.

-- *Slide* --

### Vertical scaling: an often featured support request.

Strangely, people want to keep their IP numbers...

### Q: is it worth adding info about this to the course?

Or is it too much information too soon?

-- *Slide End* --

## Lesson 8

We dive into the Object Store

It's a very simple lesson.

We introduce containers, objects, and get them upload, download and make public an image.

We also, if time permits, get them to work through connecting CyberDuck to the object store using Intersects training
material. Which needs fixing...

-- *Slide* --

### Object Store

Is it really this simple?

-- *Slide End* --

-- *Slide* --

### True or False: Knowledge is as perishable as a fresh fish!

* <span style="color:white;background:green">G</span> = True.
* <span style="color:white;background:red">R</span> = False.

-- *Slide End* --

**A** False - Is the knowledge that you have, somehow, in some strange quantum way, flipping from correct to wrong
with the passage of time?

Or is it simply that the knowledge available is exploding? Sure, some of the knowledge we may hold dear may turn out
to be incorrect (Carbohydrates are good for you?), but the majority still holds true. Pythagoras still Rulez!

## Lesson 9

We dive into Security.

We explain the shared security model, and give some basic tips on staying safe in the cloud.

This the messiest and least explored lesson, as you'll be able to tell by the lesson plan and the lesson.

-- *Slide* --

### True or False: Discovery trumps explanation

* <span style="color:white;background:green">G</span> = True.
* <span style="color:white;background:red">R</span> = False.

-- *Slide End* --

**A** True and False - Both sides have a point. If you can learn quantum physics by discovery: well, why are you
in this room? Research has shown that pure discovery learning doesn't work: but guided investigative learning can be
very effective in certain settings.
