# Hugo-Gruvbox-Theme
Simple personal blog/portfolio theme for Hugo.

Inspired by the [Ezhil](https://github.com/vividvilla/ezhil) theme and with the colors from [Gruvbox](https://github.com/morhetz/gruvbox).

## Features
- Gruvbox theme
- Minimal
- Responsive
- Supports tags
- Social Media Links
- Syntax highlighting (Gruvbox)
- Twitter cards + opengraph support
- Hugo RSS feed
- Reading Time of Posts
- Google Analytics
- Post Sharing Button
- Utterances Comments Feature support

## Demo
[View Website](https://mayadevbe.me/)
![Screenshot](images/screenshot.PNG "Gruvebox Theme")

[Erik Zaadis Blog](https://erikzaadi.com/) is now also using this theme.

## Installation
- clone
    From the Hugo-Site folder
    ```
    cd themes
    git clone https://github.com/MayADevBe/Hugo-Gruvbox-Theme.git
    ```
- download
    Unzip into the 'themes' folder

For more information checkout the [Hugo Installation Guide](https://gohugo.io/getting-started/installing/)

## Configuration
- Put a favicon in 'static\ico\favicon.svg'
- 'config.toml' example:
```toml

baseURL = "http://example.com/"
languageCode = "en-us"
title = "Website Name"
theme = "Hugo-Gruvbox-Theme"

copyright = "© Copyright Notice"

[author]
  name = "Author Name"

#Number of posts shown on index page
paginate = 5

[params]
    # Blog subtitle + For Twitter cards
    description = "A Blog about ..."
    #Google Analytics Tracking ID
    googleAnalytics = "UA-xxxxxxxxx-x"
    # Related Posts
    enableRelatedPosts = true
    relatedPostsNumber = 2
    #For Utterances Comments Feature - need to add repo
    commentRepo = "GithubName/PublicRepoName"

#Main Menu (below header)
[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All Posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 3

[[menu.main]]
name = "About"
url = "/about"
weight = 4

#Footer Menu
[[menu.footer]]
name = "Imprint"
url = "/imprint"
weight = 1

[[menu.footer]]
name = "PrivacyPolicy"
url = "/privacypolicy"
weight = 2

# Social Media Links (in header)
# Uses feather icons (search icon names on the site)
[[params.social]]
name = "Github"
icon = "github"
url = "https://github.com/MayADevBe"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://twitter.com/MayADevBe"

#enable tags
[taxonomies]
  tag = "tags"

# allow raw HTML
[markup]
  [markup.goldmark]
    [markup.goldmark.renderer]
      unsafe = true

# Syntax Highlighting
pygmentsUseClasses = true
pygmentsCodefences = true
[markup.highlight]
    codeFences = true
    guessSyntax = true
    hl_Lines = ""
    lineNoStart = 1
    lineNos = true
    lineNumbersInTable = true
    tabWidth = 4
    noClasses = false

#related config
[related]
  includeNewer = true
  threshold = 80
  toLower = true

  [[related.indices]]
    name = "tags"
    weight = 100

  [[related.indices]]
    name = "date"
    weight = 10

```

## Credits
- [Ezhil](https://github.com/vividvilla/ezhil)
- [Gruvbox](https://github.com/morhetz/gruvbox)
- [Feather Icons](https://feathericons.com/)
- [Sharing Buttons](https://sharingbuttons.io/)
- [Utterances](https://github.com/utterance/utterances)
