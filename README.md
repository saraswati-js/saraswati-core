# Alexandria Library

## Enterprise level documentation. 

![](./packages/_images/patrick-robert-doyle-OvXht_wi5Ew-unsplash.jpg)
[Photo by Patrick Robert Doyle on Unsplash](https://unsplash.com/photos/OvXht_wi5Ew)

What does this mean? Why can't there just be "documentation"? "YOU FOOL! YOU LET YOUR HUBRIS CONTROL YOU!"

## Problems of existing documentation

Documentation in:
* code should be for logic. or types.
* tests explain happy and problem paths.
* `markdown` is scattered and hard to find, if you're lucky. Also [primarily] developer focused.

## The solution space
Alexandria seeks to fix this problem by using convention (then configuration) to build documentation from many disparate repos and compiling into one source.

To do this we use an extended Markdown to allow for flexibility and configuration on the target repo to build content as needed for a static site.

So now documentation is updated closer to the behavior that it's describing. There is now no reason to not keep things up to date. Everything can be organized/grouped easily w/o having to do a lot of configuration by the dev or an administrator.

## Features
Note: You can use it as a regular static website builder but it's a little over powered for that. On the plus side it'll have a lot of the same features of the [GatsbyJS docs](https://www.gatsbyjs.org/docs) site.

### Overview
1. Have hundreds of repos with markdown in them, pull them into a central repository and build documentaiton with those file and build relationships between documents.
1. Have a single store for all your architecture documents.
1. Build links to all repo important items.
1. Have a React component playground using markdown.

### Documentation
#### General Docs
1. Table of contents
1. Sidebar is based on `markdown` front-matter
1. Configurable (edit on github, delta for dynamic sorting, )
1. Lots of `markdown` plugins to expand the functionality of `mdx`.
1. Versioning, changelogs, et al.
1. Index pages of all your content.
1. Platform links and documents are organized by `frontmatter`.

#### Playground
1. Like storybook but easier.
1. Have access to A11Y tools.
1. Prop toggles.
1. Prop documentation.

#### Architecture
1. Diagrams out the wahzoo!
1. Build relationships between all the content. Interlink, use content from them (snippets, etc)
    - Imagine writing a part of your architecture and not having to do it all in one place! Instead you build relationships in your documentation in the `frontmatter` (all showed in the main site as a link) and then have it all compiled together later!
1. Embed repo specific code into any markdown file.

#### Guides / Tutorials
1. Build a wizard of content to guide people through the use of content
1. Checkboxes to let people keep track of their own progress.
1. Great to use for self onboarding for new employees.

#### Glossary
1. Create terms in-line to your documentation and build a glossary to a specific page, inline at the bottom or elsewhere.
1. Add to the glossary specifically
1. Add aliases and terms to existing terms. Sometimes there is a bunch of jargon and this will make it easier.

#### Server & Tools
1. Local runner to show off your docs or use a component playground.
1. A server and DB to manage building of everything (best for pipelines).
1. Notifiers so that people can subscribe to documentation changes.

All documentation can now stay up to date (devs can't point fingers anymore).

## Packages
_All of this is subject to change; it's just the way that I see it at 12:05PM on 30/01/2020_

If optional is `Y` an administrator can add these packages at their discretion. Otherwise it's required by another package to be used.

### End user
These are the packages/repos that you'd use to setup a site. 

|  Package | Description | Configurable? | Optional? |
|---|---|---|---|
| `@alexandria/theme` | |   | `N` | 
| `@alexandria/example-site` | | Highly, this shows off ALL the features | `Y` | 
| `@alexandria/local-runner` | | Add as a dev dep to run in your package locally | `Y` | 
| `@alexandria/cli` | | Install globally to use tools to run your site (Gatsby) and your local site or to add `@alexandria` functionality to an existing repo  | `Y` | 

### End user - Optional
|  Package | Description | Configurable? | Optional? |
|---|---|---|---|
| `@alexandria/api-code` | JS Docs in your code | `Y`  | `Y` | 
| `@alexandria/api` | Swagger in my docs? Heck yes! | `?` | `Y` | 
| `@alexandria/architecture` | Communal based archiecture docs based on product or just on a page |  `Y` | `Y` | 
| `@alexandria/changelog` | |   |  | 
| `@alexandria/glossary` | |   | `N` | 
| `@alexandria/guide` | |   | `N` | 
| `@alexandria/info` | |   | `Y` | 
| `@alexandria/playground` | |   | `Y` | 
| `@alexandria/versioning` | |   | `Y` | 
| `@alexandria/publisher` | |   | `Y` | 

### Dependancies
ie: These are required by any/all of the "End User" packages above.

|  Package | Description | Configurable? | Optional? |
|---|---|---|---|
| `@alexandria/components` | |   | `N` | 
| `@alexandria/core` | |   | `N` | 
| `@alexandria/dewey` | |   | `N` | 
| `@alexandria/docs` | |   | `N` | 
| `@alexandria/layouts` | |   | `N` | 
| `@alexandria/remark` | |  `N` | `N` | 
| `@alexandria/repos` | |   | `N` | 

## Examples
Examples in `./packages/@alexandria/example-site`. Change config in `gatsby-config.js` and remove repos to show docs coming from remote repos or just what is contained in the folder `./packages/alexandria-example-site`.
