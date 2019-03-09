# project-checklist

A Checklist for Good Projects

* Initial presentation
    * This is usually the README of your project
    * Do not list out all the functionalities of your project as the first thing in the README
        * Showing users all the options they can do with something will confuse them
            * Example
            * The first example you show should be the absolute most basic example that is working and copy-and-paste-able. 
            * My definition of simplicity: something is simple when there is nothing left to take away from it
            * Don’t initially show users multiple ways of doing something. Show them only one way of doing it. Be careful which way you show them. Choose the way that will most use most of the time
        * It’s tempting to show your users all the things they can do with your project. In many cases, however, this will intimidate users (especially those that are new to the idea or the ecosystem)
    * Start by showing the most common functionalities first
    * Should include some kind of live demo
        * Examples
            * lint-staged
            * eslint-plugin-compat
        * asciinema.org is recommended to record these
        * Examples should be interactive as well. Consider using codesandbox to provide live and runnable demos
* Code Conventions
    * Don’t use meaningless variable names, examples
        * Provide examples at are going to be similar to what users will use your library for
        * If you are making an assertion library, don’t make examples like so:
            * Bad: foo = checkIsUsername(a)
            * Better: username = checkIsUsername(user.username)
    * All examples should be standalone
        * A lot of users copy and paste examples just to see if they can get your project working. Having examples that can be copy and pasted and gotten working will lower the barrier to new users.
        * In projects are too complex to have standalone examples, at the least they can have standalone environments that they can run their examples in. Docker, for example, can be used to implement this well. Users can spin up a docker container and run their examples in the container instead of spending time getting their own environment set up
* Project Quality
    * Be your own user. If you’re making a library, build an app that uses it. See what you like and dislike about your library from the perspective of a user.
    * Before MVP, all tests should be passing and docs with examples should be written and made available
* Branding
    * Make your project unique and memorable (most people only focus on technical aspects of a project). While this is important, this should be done close to finishing the MVP of a project
    * Naming your project
        * Name your project something that is easy to remember
        * Try to make the name related to what you’re making
            * Examples:
                * “parcel” is the name of a bundler
                * “React” comes from reactive programming
                * “Flow” comes from flow graph inference
        * Single words or combining common words
            * Examples: React, ”micro-soft“, ”face-book“, ”web-pack“, ”flow“, etc
        * Don’t worry too much about choosing a name and having a package with that name already take. If your project becomes more popular than the project that has taken the name already, the owner of the package will usually give you the package name if not too many people are depending on it
    * Add a logo
        * Make sure your logo is one of the first things your audience sees when they see your project
        * Don’t use letter logos. Use images or icons that are similar to your project. For example, if your project is called joker, add a picture of a joker card instead of simply creating a logo with the word “joker”
        * Easily compress your logo with Squoosh
    * Choose a color theme
        * React’s is blue and light blue
        * Flow’s is yellow and gray
        * Make sure your docs and website follow this color theme
    * Further reading
        * If you want to learn more about marketing, see LisaDziuba/Marketing-for-Engineers
* Optional
    * Related sections
        * Listing projects that are related to your projects can help users with discovering other related projects
        * This is mostly for the purpose of spreading awareness and improving the connectedness of the community
        * For each project you list, provide the name of the project and a short description of it
* Onboarding Methods
    * Provide the most “native” ways of on boarding people
