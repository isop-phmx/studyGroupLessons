# Pharmacometrics Study Group Lessons

Let's build a collection of introductory lessons for short tutorials on scientific coding, writing, data management and anything else connected to open science, that people can deliver to a Study Group in their labs and departments.

### What's a Pharmacometrics Study Group and How do I Start One?

Pharmacometrics Study Groups are fun, informal meetups of your friends and colleagues from around your local institution or town to share skills, stories and ideas on using code for research. The goal is to create a friendly, no-pressure environment where people can share their work, ask for help on a coding problem or learn new concepts or discuss new advances in our field, and learn and work together with their peers.

### What is a Study Group Lesson Like?

A good Study Group lesson should be a tutorial that's *as hands on as possible* - an hour-long lecture just doesn't have the same effect. To create a successful tutorial, keep the following in mind:

 - Give participants challenge questions to try out their new skills as often as possible; never lecture for more than five minutes at a stretch.
 - Go as slow as the participants need; never rush to get through all the material.
 - Encourage people to work together and chat about what they're learning and how they might use it.
 - Try to come up with examples that are relevant and interesting from your field of study.

Have a look in the template directory of this repository for some more details.

### Contribution Guidelines

If you'd like to contribute a new lesson, write it up in a new repo following these guidelines:
 - put the lesson script in `README.md`, with your name, subject area and lesson topic at the top.
 - make sure to include an open source `LICENSE` file.
 - make sure all data / examples / figures / anything else you want are all included in your repo.
 - Here's an [example](https://github.com/BillMills/pythonPackageLesson) of all that.

Then, add your repo to this one as a Submodule.

#### Using Submodules

Submodules are super handy for making a loose federation of resources like these, but are relatively rarely used; here's a primer.

##### Adding a new lesson

In this repo, do

```
git submodule add <url of your new lesson repo> <name to use for this lesson>
```

then commit, push and pull request as usual. That's it! Please prefix the name of the submodule with the relevant language or technology, like `R-`, `python-` etc.

##### Pulling down lessons locally

Clone this repo as usual:

```
git clone https://github.com/isop-phmx/studyGroupLessons
```

You'll see directories for all the different lessons, but they'll be empty. Tell git you're going to be using submodules (only need to do this once for this project):

```
git submodule init
```

Then, you can pull down individual submodules like so (replace `awk-lesson` with the name of the submodule you want):

```
git submodule update awk-lesson
```

Finally, pull down new changes to lessons in future via:

```
git pull upstream master
git submodule update awk-lesson
```

##### Updating Submodule Pointers

(Note: maintainers of this repo will do this automatically regularly - contributors shouldn't need to do this)

```
git submodule update --remote
```

#### Need Help?

**Not comfortable with Markdown or Git?** That's ok! If Markdown isn't your thing, just cut and paste your notes into a plain text file, and we'll help you format them; if you're unsure of git, open a new [issue](https://github.com/isop-phmx/studyGroupLessons/issues) and we'll help get you included.
