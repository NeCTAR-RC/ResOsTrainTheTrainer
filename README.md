## Git

If you check this repository out be aware that it uses Git submodules to manage the reveal.js dependency.
To also checkout reveal.js, you will have to either:

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

Remember to always walk through your slides when you regenerate them!
