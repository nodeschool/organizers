organizers 
==========

[![Gitter chat](https://badges.gitter.im/nodeschool/organizers.png)](https://gitter.im/nodeschool/organizers)

- Learn to run an event and get pro-tips from other organizers in the [organizers wiki](https://github.com/nodeschool/organizers/wiki)
- Ask a question or browse discussions in the [organizers discussion board](https://github.com/nodeschool/organizers/issues)

If you are an existing organizer, or intend to become one in the future **please read and abide by our [code of conduct](https://github.com/nodeschool/organizers/blob/master/code_of_conduct.md)**.

## How to start a new NodeSchool chapter

**First, open an issue on this repo asking to get added as a chapter organizer**

Your issue should say something like this (not everything is required but it's nice to tell us a little about yourself so you don't come across as a total stranger):

*
Hi, I would like to start a nodeschool chapter for [name of geographic community]. I am [@your twitter name] on twitter and work at/on <name of company or project>. I will be co-organizing this chapter with [names of other organizers]. I have been using Node.js for 6 months and would like to help others learn as well.
*

The chapter name should preferably be the name of the city, where the workshops will
be held. Alternatively the area should be small, but yet meaningful, e.g `princeton` instead of
`new-jersey` or `usa`. Also the repo name should be short and all lowercase.

**An existing Owner will have to respond and create your Chapter repository for you**

Once you are an organizer follow these instructions to set up your NodeSchool chapter:

### 1

You should have been added to the team called `chapter-organizers` and should have access to edit the new chapter repo, e.g. https://github.com/nodeschool/berlin

### 2

Each chapter can set up their own gh-pages branch on their org and github pages will automatically route `nodeschool.io/<reponame>` to it

For example we have [Oakland](https://github.com/nodeschool/oakland) and [Berlin](https://github.com/nodeschool/berlin).

@finnp forked the csvconf website and set up [a gh-pages branch](https://github.com/nodeschool/berlin/tree/gh-pages) for the berlin repo and thanks to the awesomeness that is GitHub Pages this url automatically works: http://nodeschool.io/berlin/

You should create a code of conduct for your website and repository. You can use 
[this template](codeofconduct-template.md) as a starting point. Make sure to make
all people feel welcome at your event.

Another bonus feature is that you can simply use `gitter.im/nodeschool/<chaptername>` to automatically get a chat room for your chapter.

### 3

_This step is important for discoverability!_

Once your chapter is up and running, make a pull request to the [NodeSchool website](https://github.com/nodeschool/nodeschool.github.io/) to add a chapter JSON file to the /chapters directory. Before submitting your pull request, ***do not forget*** to run `npm build` to update all the appropriate json files. When your request is accepted, your chapter will get auto-added to http://nodeschool.io/chapters.html

The chapter JSON file should look something like this: 

```json
{
  "name": "Baltimore NodeSchool",
  "location": "Baltimore, MD",
  "country": "US",
  "region": "North America",
  "organizers": ["jasonrhodes"],
  "website": "http://nodeschool.io/baltimore",
  "twitter": "bmorenodeschool",
  "repo": "http://github.com/nodeschool/baltimore"
}
```

**Chapter JSON field info:**

| field | description |
|-------|-----------|-------------|
| `name`* | Whatever you call your event, often `<location> NodeSchool` |
| `location`* | This appears on the chapters.html page, often `<City>` or `<City, State>` but can be any geocode-able string |
| `country` | If your location isn't a country, list the [ISO-3166 2-letter country code](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) for consistency |
| `region`* | Choose an existing region from [the chapters page](http://nodeschool.io/chapters.html) if possible--if not then pick a broad, non-country region name |
| `organizers` | An array of GitHub usernames |
| `website` | URL to the main website for your chapter, if one exists besides your GitHub repo |
| `repo`* | GitHub repo URL |
| other? | Any other services like Twitter, Gitter, etc. that exist for the _chapter_ (not the organizer's info) |

*required

---

That's all the mandatory steps. Here are some optional steps:

#### Add your events to the NodeSchool webpage

Fill out this [form](https://docs.google.com/forms/d/1vYW-Yw82kt_q7WDgBY6gQqFrg3zuD2rDPXEG-cbq7e4/viewform?usp=form_confirm) to add your event to the website.

#### Make a logo

You can [use this .AI/.SVG template](https://github.com/nodeschool/nodeschool.github.io/tree/master/images/make-a-sticker) to design your own custom nodeschool sticker/logo. There is also a [design helper](http://www.finnpauls.de/nodeschool-stickerify/) for the browser based on the design for sketching a simple sticker.


### Benefits of this approach

- chapters get their own "mailing list" (github issues). These can be in other languages as well, e.g. Spanish for Latin-American Chapters, whereas the main Discussions repo is primarily in English
- all NodeSchool attendees leave with a GitHub account and a community they can ask questions to
- chapters get their own website
- since all chapter members are [open open source](https://github.com/rvagg/node-leveldown#contributing) style contributors it means everyone gets empowered to help moderate discussions and improve the chapter website
- we can list all of the chapters on the nodeschool site
