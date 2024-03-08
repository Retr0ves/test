# D.O.C.C. Lab Website

Welcome to the repository for the D.O.C.C. Lab website.

<!-- ## Lighthouse PageSpeed Insights

[![Google PageSpeed](https://raw.githubusercontent.com/alshedivat/al-folio/master/assets/img/pagespeed.svg)](https://pagespeed.web.dev/report?url=https%3A%2F%2Falshedivat.github.io%2Fal-folio%2F&form_factor=desktop) -->

<!-- ## Table Of Contents

- [al-folio](#al-folio)
  - [User community](#user-community)
  - [Lighthouse PageSpeed Insights](#lighthouse-pagespeed-insights)
  - [Table Of Contents](#table-of-contents)
  - [Getting started](#getting-started)
  - [Installing](#installing)
  - [Customizing](#customizing)
  - [Features](#features)
    - [Light/Dark Mode](#lightdark-mode)
    - [CV](#cv)
    - [People](#people)
    - [Publications](#publications)
    - [Collections](#collections)
    - [Layouts](#layouts)
      - [The iconic style of Distill](#the-iconic-style-of-distill)
      - [Full support for math \& code](#full-support-for-math--code)
      - [Photos, Audio, Video and more](#photos-audio-video-and-more)
    - [Other features](#other-features)
      - [GitHub's repositories and user stats](#githubs-repositories-and-user-stats)
      - [Theming](#theming)
      - [Social media previews](#social-media-previews)
      - [Atom (RSS-like) Feed](#atom-rss-like-feed)
      - [Related posts](#related-posts)
  - [FAQ](#faq)
  - [Contributing](#contributing)
    - [Maintainers](#maintainers)
    - [All Contributors](#all-contributors)
  - [License](#license) -->

## Installing

For instalation details please refer to [INSTALL.md](INSTALL.md).

## Theme

This website is using a color palette consisting of 6 colors. The colors are used for different elements of the website, such as the background, text, links, and more. The colors are defined in the `_sass/variables.scss` file. The colors are defined as CSS variables, so they can be easily reused throughout the website.

![Color Scheme](assets/img/readme_preview/colors.svg)

- **Primary**: #482BE7 
- **Secondary**: #25DAC5
- **Contrast**: #E93A7D
- **Background**: #FFFFFF
- **Text**: #151439
- **Heading**: #1E0E62

## Customizing

### Navigation Bar

The navigation bar is generated automatically based on the pages in the `_pages` directory. The order of the pages in the navigation bar is determined by the `nav_order` attribute in the page's front matter. The navigation bar can be customized by adding or removing pages from the `_pages` directory and by changing the `nav_order` attribute in the front matter of the pages.

To add a link to an external page in the navigation bar, add `external_link` to the front matter of the page and set it to the URL of the external page.

You can also hide an item from the navigation bar by setting `nav: false` in the front matter of the page.

### News

The news section is generated based on the posts in the `_news` directory. The items are ordered by date, with the most recent item appearing first.

### Projects
#### Projects Page
Each project page is consists of four main sections:
- **Header**: The header section contains the title of the project and the project's description which is generated based on the project's front matter.
- **Content**: The main content.
- **Related Publications**: The related publications section is generated based on the `related_publications` attribute in the project's front matter. The value of the `related_publications` attribute is the publication's key in the `_bibliography/paper.bib` file.

  For instance, if you want to refer to the publication in the bib file:
  ```bibtex
  @inproceedings{Sambasivan:2017jb,
    author = {Sambasivan, Raja R. and Tran-Lam, David and Akella, Aditya and Steenkiste, Peter}, 
    title = {Bootstrapping evolvability for inter-domain routing with D-BGP}, 
    ...
  }
  ```
  You would add the following to the project's front matter:
  ```yaml
  related_publications: alshamali2021
  ```
  If you have multiple publications, you can add them as a list separated by a comma.

- **People**: The people section contains the people involved in the project. 
  The people are generated based on the `team` attribute in the project's front matter. The value of the `team` attribute is a list of people involved in the project. Each person is represented as a yaml list item with the following attributes:
  - `name`: the name of the person
  - `image`: the path to the image file
  - `role`: the role of the person

  For instance, if you want to add a person to the project:
  ```yaml
  team:
    - name: Raja Sambasivan
      image: raja_sambasivan_resized.png
      role: Assistant Professor, Tufts University
  ```

  The images of profiles should be placed in the `assets/img/people` directory.
#### Selected Projects
The selected projects section on home page is generated based on the projects in the `_projects` directory with the `selected: true` attribute in the front matter. 

### Fun/Events

The fun page is a photo gallery that can be customized by adding or removing images from the `_pages/fun.md` file. Each image is represented a yaml list item with the following attributes:
- `src`: the path to the image file
- `title`: the title of the image
- `description`: a description of the image
- `date`: the date the image was taken
- `link`: a link to a page with more information about the image

The order of the images in the gallery is determined by the order of the yaml list items in the `_pages/fun.md` file.

### People/Profiles

Profile page has three main sections: members, friends of the lab, and alumni. Each section is generated according to the items in fields `members`, `friends`, and `alumni` in the `_pages/profiles.md` file. Each item is represented as a yaml list item with the following attributes:
- `name`: the name of the person
- `image`: the name of the image file, the image should be placed in the `assets/img/people` directory
- `interests`: the interests of the person, separated by a comma
- `role`: the role of the person
- `link`: the link to the person's website, if available

For any other customization details please refer to [CUSTOMIZE.md](CUSTOMIZE.md).




