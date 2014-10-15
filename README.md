organizers 
==========

[![Gitter chat](https://badges.gitter.im/nodeschool/organizers.png)](https://gitter.im/nodeschool/organizers)

A discussion repository for nodeschool organizers

## How to start a new NodeSchool chapter

**First, open an issue on this repo asking to get added as an Owner**

Your issue should say something like this (not everything is required but it's nice to tell us a little about yourself so you don't come across as a total stranger):

```
Hi, I would like to start a nodeschool chapter for <name of geographic community>. I am <@your twitter name> on twitter and work at/on <name of company or project>. I will be co-organizing this chapter with <names of other organizers>. I have been using Node.js for 6 months and would like to help others learn as well.
```

Once you are an owner follow these instructions to set up your NodeSchool chapter:

### 1

Chapter owner should create a repo for their chapter, e.g. https://github.com/nodeschool/berlin

### 2

Chapter owner should make a new Team on the nodeschool org with the same name. The owner then has to go into the chapter org and specifically add the chapter team as a collaborator:

![screen shot 2014-08-21 at 2 44 41 pm](https://cloud.githubusercontent.com/assets/39759/4004063/751d878c-297c-11e4-9101-d22a9d7ff037.png)

### 3

**Everyone** who ever attends a nodeschool event by that chapter should added as a member of the chapter team by the Owner (so they can open/close issues and push to the chapter org but can't e.g. delete repos). People can obviously decline the invitation to get added.

A note on github orgs: Only Owners can add new team members. The original Owner can add other trustworthy people from the chapter to the Owners team so that they can also add NodeSchool attendees to your chapter's team. Please use good judgment when adding new Owners, as Owners also have the ability to delete other chapter's repositories. 

### 4

Each chapter can set up their own gh-pages branch on their org and github pages will automatically route `nodeschool.io/<reponame>` to it

For example we have [Oakland](https://github.com/nodeschool/oakland) and [Berlin](https://github.com/nodeschool/berlin) repos now, and I made [corresponding teams](https://github.com/orgs/nodeschool/teams)

@finnp forked the csvconf website and set up [a gh-pages branch](https://github.com/nodeschool/berlin/tree/gh-pages) for the berlin repo and thanks to the awesomeness that is GitHub Pages this url automatically works: http://nodeschool.io/berlin/

Another bonus feature is that you can simply use `gitter.im/nodeschool/<chaptername>` to automatically get a chat room for your chapter.

### 5

Once your chapter is up and running, make a pull request to the [NodeSchool website](https://github.com/nodeschool/nodeschool.github.io/) Chapters page to add your Chapter to the directory

That's all the mandatory steps. Here are some optional steps:

#### Add your events to the NodeSchool webpage

Fill out this [form](https://docs.google.com/forms/d/1vYW-Yw82kt_q7WDgBY6gQqFrg3zuD2rDPXEG-cbq7e4/viewform?usp=form_confirm) to add your event to the website.

#### Make a logo

You can [use this .AI/.SVG template](https://github.com/nodeschool/nodeschool.github.io/tree/master/images/make-a-sticker) to design your own custom nodeschool sticker/logo. There is also a [design helper](http://www.finnpauls.de/nodeschool-stickerify/) for the browser based on the design for sketching a simple sticker.


### Benefits of this approach

- chapters get their own "mailing list" (github issues). These can be in other languages as well, e.g. Spanish for Latin-American Chapters, whereas the main Discussions repo is primarily in English
- all NodeSchool attendees leave with a GitHub account and a community they can ask questions to
- chapters get their own website
- chapters can start quantifying their membership
- chapters can get pinged using `@nodeschool/<teamname>`
- since all chapter members are [open open source](https://github.com/rvagg/node-leveldown#contributing) style contributors it means everyone gets empowered to help moderate discussions and improve the chapter website
- we can list all of the chapters on the nodeschool site
