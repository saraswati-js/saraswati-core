# Alexandria Library

Enterprise level documentation. 

Generate documentation for many repos or just one site's documentation for self.

![](./packages/_images/patrick-robert-doyle-OvXht_wi5Ew-unsplash.jpg)
[Photo by Patrick Robert Doyle on Unsplash](https://unsplash.com/photos/OvXht_wi5Ew)

## Packages
_All of this is subject to change; it's just the way that I see it at 12:05PM on 30/01/2020_

If optional is `Y` an administrator can add these packages at their discretion. Otherwise it's required by another package to be used.

### End user
These are the packages/repos that you'd use to setup a site. 

|  Package | Description | Configurable? | Optional? |
|---|---|---|---|
| `alexandria-theme` | |   | `N` | 
| `alexandria-example-site` | | Highly, this shows off ALL the features | `Y` | 

### End user - Optional
|  Package | Description | Configurable? | Optional? |
|---|---|---|---|
| `alexandria-api-code` | JS Docs in your code | `Y`  | `Y` | 
| `alexandria-api` | Swagger in my docs? Heck yes! | `?` | `Y` | 
| `alexandria-architecture` | Communal based archiecture docs based on product or just on a page |  `Y` | `Y` | 
| `alexandria-changelog` | |   |  | 
| `alexandria-glossary` | |   | `N` | 
| `alexandria-guide` | |   | `N` | 
| `alexandria-info` | |   | `Y` | 
| `alexandria-playground` | |   | `Y` | 
| `alexandria-versioning` | |   | `Y` | 

### Dependancies
ie: These are required by any/all of the "End User" packages above.

|  Package | Description | Configurable? | Optional? |
|---|---|---|---|
| `alexandria-components` | |   | `N` | 
| `alexandria-config` | |   | `N` | 
| `alexandria-core` | |   | `N` | 
| `alexandria-docs` | |   | `N` | 
| `alexandria-layouts` | |   | `N` | 
| `alexandria-remark` | |  `N` | `N` | 
| `alexandria-repos` | |   | `N` | 

## Examples
Examples in `./packages/alexandria-example-site`. Change config in `gatsby-config.js` and remove repos to show docs coming from remote repos or just what is contained in the folder `./packages/alexandria-example-site`.
