## Titus Theming
This is an example theme for RSC Titus v3.0. Read below for theming documentation.

## Theme Requirements
To apply a theme to Titus, it *must* have these requirements:

- A unique folder/repository name. This can be anything, so long as it conforms to unix file naming specifications and contains *no* whitespace. (For example, `gentlemen`)
- A valid `theme.yml` file containing the correct configuration information.
- An `index.html` file containing the markup for the theme.
- A `lib/` directory. This is where *all* CSS, Javascript and general assets are to be placed.

All of the above should exist in the root directory of the theme.

## Theme.yml
Required parameters are as follows: 
- `name`
- `description`
- `slug` - This **MUST** be exactly the same as the directory name. 

Use [this file](https://github.com/jonlambert/rsc-example-theme/blob/master/theme.yml) as an example `theme.yml`.

## Tags

|Tag                  |Usage                                                                                                    |
|---------------------|---------------------------------------------------------------------------------------------------------|
|`<!-- @framework -->`|Bootstraps all of the Javascript features in Titus. Place this right before `</head>`.                   |
|`<!-- @source -->`   |Injects the lazy-loading Javascript files. Place before `</body>`.                                       |

As with `theme.yml` you can use [this file](https://github.com/jonlambert/rsc-example-theme/blob/master/index.html) as an example `index.html`.
