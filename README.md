# Alexandria Library

Enterprise level documentation. 

What does this mean? Why can't there just be "documentation"? "YOU FOOL! YOU LET YOUR HUBRIS CONTROL YOU!"

Documentation is just documentation and this is great but there are issues with how documentation in groups. Most enterprises do not organize their documentation properly nevermind doing it well. It's scattered and isn't maintained. The best place to put most of your documentation is within the code itself. Unfortunatly there is a lot of debate on this. Some will do it as Markdown, some as comments, others as unit tests. All work but aren't great.

* Documentation in code should be for logic.
* Documentation in tests is to explain how to use code.
* Documentation in Markdown is great because it's simple and is often up-to-date but lives only in the repo.

The solution is to do everything in markdown because it's syntax is simple [and extendable] but the main issue is still that this documentaiton lives in the code. The other issue is that it you need to go to a repo (if you know where it is) to get that information. It's also not linked together. It's completely separated from everything else. How to fix this?

Keep everything in the repo but publish elsewhere. Keep everything separated in any place but have a tool _build_ your documentation. Do your organization of content on a markdown file basis and set up relationships between your archiecture anywhere.

The solution is to generate documentation for many repos or just one site's documentation for self.

![](./packages/_images/patrick-robert-doyle-OvXht_wi5Ew-unsplash.jpg)
[Photo by Patrick Robert Doyle on Unsplash](https://unsplash.com/photos/OvXht_wi5Ew)

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
