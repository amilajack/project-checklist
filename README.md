![logo](logo.png)

<h1 align="center">project-checklist</h1>
<h3 align="center">A checklist of things to do before releasing your project</h3>


> ### The best projects sell themselves


## 🎨 Initial Presentation

Think of the `README` as the elevator pitch for your project. Keep it concise and to the point

- [x] Don't list out all the functionalities of your project as the first thing in the `README`
  * Recommendations
    * Showing users all the options they can do with something will confuse and/or overwhelm them
    * The first example you show should be the absolute most basic example that is working and copy-and-paste-able. 
    * My definition of simplicity: something is simple when there is nothing left to take away from it
    * Don’t initially show users multiple ways of doing something. Show them only one way of doing it. Be careful which way you show them. Choose the way that will most use most of the time
    * It’s tempting to show your users all the things they can do with your project. In many cases, however, this will intimidate users (especially those that are new to the idea or the ecosystem)
- [x] Start by showing the most common functionalities first. If your project is an API, only initially show examples of the most common APIs that are used. If your project is an app, show screenshots of the pages that are most commonly used
- [x] Include a live demo. A video is a thousand pictures and a picture is a thousand words
  * Recommendations
    * [asciinema.org](https://asciinema.org) is recommended to record these
  * Examples
    * [lint-staged](https://github.com/okonet/lint-staged#-lint-staged----)
    * [eslint-plugin-compat](https://www.github.com/amilajack/eslint-plugin-compat#eslint-plugin-compat)
- [x] Communicate your [Value Proposition](#value-proposition)
- [x] Provide interactive examples. Having ready and runnable examples lowers the barrier to using and testing out your project
  * Recommendations
    * General Programs: consider using [replit](http://repl.it) to provide live and runnable demos
    * Web Libraries: consider using [codesandbox](https://codesandbox.io) to provide live and runnable demos. For [node](https://nodejs.org), consider running them in [runkit](https://runkit.com)
    * Web Apps: Provide links to the hosted version of your app

## 💰 Value Proposition

> A value proposition is a promise of value to be delivered, communicated, and acknowledged

Figure out the value your project brings to your users. What does it provide them that they don't have already? 

* Examples
  * [React](https://github.com/facebook/react): Declarative, efficient, easy to use
  * [Babel](https://github.com/babel/babel): Easy-to-use, pluggable
  * [Yarn](https://github.com/yarnpkg/yarn): Performance, ergonomics, reproducible installs

* Recommendations
  * A value proposition can have multiple propositions
  * [Writing down a market positioning statement](http://blog.ecornell.com/how-to-write-market-positioning-statements/) or statements can help with clarity, business goals, marketing and more
  * Having better performance than competing projects usually isn't enough to convince people to use your project. If you are using better performance as your only value proposition, consider adding other value propositions (see [the tweet](https://twitter.com/sebmck/status/1105189411690405892)).

- [x] Decide what your value proposition is
- [x] Communicate your value proposition in your `README` and in your tagline

## 💯 Project Quality

High quality projects are much more likely to retain users over time

- [x] Be your own user. If you’re making a library, build an app that uses it. See what you like and dislike about your library from the perspective of a user
- [x] Before [MVP](https://en.wikipedia.org/wiki/Minimum_viable_product) (minimum viable product), all tests should be passing and docs with examples should be written and made available

## 👑  Branding

Make your project unique and memorable (most people only focus on technical aspects of a project). While this is important, this should be done close to finishing the MVP of a project

- [x] Name your project
  * Recommendations
    * Name your project something that is easy to remember
    * Try to make the name related to what you’re making
      * Examples
        * [Parcel](http://parceljs.org): “parcel” is the name of a bundler
        * [React](http://reactjs.org): “React” comes from reactive programming
        * [Flow](https://flow.org): “Flow” comes from flow graph inference
    * Single words or combining common words
      * Examples
        * React
        * ”micro-soft“
        * ”face-book“
        * ”web-pack“
    * Don’t worry too much about choosing a name and having a package with that name already take. If your project becomes more popular than the project that has taken the name already, the owner of the package will usually give you the package name if not too many people are depending on it
- [x] Add a tagline
  * Recommendations
    * Avoid wordy taglines--they are hard to remember and understand
    * Your tagline should communicate your value proposition
  * Examples
    * [React](https://github.com/facebook/react): A declarative, efficient, and flexible JavaScript library for building user interfaces
    * [Babel](https://github.com/babel/babel): The compiler for writing next generation JavaScript
    * [Yarn](https://github.com/yarnpkg/yarn): Fast, reliable, and secure dependency management for JavaScript
- [x] Add a logo
  * Recommendations
    * Make sure your logo is one of the first things your audience sees when they see your project
    * Don’t use letter logos. Use images or icons that are similar to your project. For example, if your project is called joker, add a picture of a joker card instead of simply creating a logo with the word “joker”
    * Easily compress your logo with Squoosh
- [x] Choose a color theme
  * Examples
    * React’s is blue and light blue
    * Flow’s is yellow and gray
    * Make sure your docs and website follow this color theme
- [x] Further reading
  * If you want to learn more about marketing, see [LisaDziuba/Marketing-for-Engineers](https://github.com/LisaDziuba/Marketing-for-Engineers)

## ✈️ Entry Barriers

Lower the barrier to entry by providing the most “native” ways of on boarding people. Make it as easy as possible for users of competing projects to start using your project.

In general, here's how this works: say you have library `y` that competes with popular libray `x`, write documentation for a migration path from library `x` to `y`.

* Examples
  * [Figma](http://figma.com), a vector graphics editor, gained users by allowing [Sketch](http://sketchapp.com) users to import Sketch files into Figma
  * [Laravel](http://laravel.com) onboarded many [Rails](https://rubyonrails.org) users by providing terminology and conventions that were similar to [Rails](https://rubyonrails.org)

In general, you can't expect your users to _engage_ in your project if the barriers are as high for them as they were for you as the original developer. Here are some additional ideas:

* Can your development environment be _easily_ replicated by your users?
* Can they build your software and get started as easily as you can as the upstream developer?
  * Think cross-platform: can someone on a Mac, or Linux, or Windows Subsystem for Linux build and use your software? And do you show the build status for all of those platforms?
  * What about someone doing that in a VM? Or a container? Or a different version of Python? Or with no `sudo` access?
* How will users get your bits, and how will they keep them updated? For libraries, this is "easier" (npm, pypi, etc.) but often times users can benefit from other methods including native packages, Homebrew or in some cases even `curl | sh`.

## 🧹 Code Conventions and Infrastructure

Using standard code conventions and infrastructure lowers the barrier for people that want to contribute to your project. This sometimes translates to more contributors over time because initial contributors sometimes become long term contributors

- [x] Don’t use meaningless variable names or examples
- [x] Provide examples at are going to be similar to what users will use your library for
- [x] If you are making an assertion library, don’t make examples like so:
  - [x] Bad: foo = checkIsUsername(a)
  - [x] Better: username = checkIsUsername(user.username)
- [x] All examples should be standalone
- [x] A lot of users copy and paste examples just to see if they can get your project working. Having examples that can be copy and pasted and gotten working will lower the barrier to new users
- [x] In projects are too complex to have standalone examples, at the least they can have standalone environments that they can run their examples in. Docker, for example, can be used to implement this well. Users can spin up a docker container and run their examples in the container instead of spending time getting their own environment set up

## ️📣 Spread the Word

* General Projects
  - [x] Submit project to [Changelog News](https://changelog.com/news/submit)
  - [x] Submit project to [Hacker News](https://news.ycombinator.com/submit)
  - [x] If web related, submit to [dev.to](https://dev.to)
  - [x] Post on [twitter](https://twitter.com) and upload images of project
  - [x] Post to corresponding reddit programming language community [/r/javascript](https://www.reddit.com/r/javascript), [/r/python](https://www.reddit.com/r/python), etc
  - [x] When appropriate, consider [talking about your project publicly](https://github.com/vmbrasseur/Public_Speaking)

* Specific for Apps / Products
  - [x] Submit project to [Product Hunt](https://www.producthunt.com)

To maintain communication with existing users, use a newsletter. Consider using [mailchimp](https://mailchimp.com) for this. Be aware that once communication becomes more fluid, you might create support expectations so it becomes critical to [understand open source support systems](https://nadiaeghbal.com/user-support).

## 🤑 Funding

<!-- TODO: Discussion on business models, probably bringing lemonade-stand up here. -->

* [Open Collective](https://opencollective.com): Ideal for large projects with many users
* [Patreon](http://patreon.com): Ideal for developers with many projects
* [Issue Hunt](https://issuehunt.io): Ideal for popular projects with many users and high priority bugs
* More details
  * [oss.cash](http://oss.cash) for a comprehensive list of funding mechanisms
  * [lemonade-stand](https://github.com/nayafia/lemonade-stand)

## Optional

- [x] Mention Related Projects
  * Listing projects that are related to your projects can help users with discovering other related projects
  * This is mostly for the purpose of spreading awareness and improving the connectedness of the community
  * For each project you list, provide the name of the project and a short description of it
  * Examples
    * [sindresorhus/p-throttle](https://github.com/sindresorhus/p-throttle#related)
