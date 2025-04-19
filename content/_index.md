---
title: About
catchline:
gmaps: false
---

# TEST ABOUT PAGE

## Demo

## Installation

### As Git Submodule

## Usage

### Edit your config file

### Customize main color

### Set Google Maps url

In your config file, add:

``` yaml
params:
  gmaps_url: https://tinyurl.com/mr3uesbx
```

### Image Gallery

#### Use as partial

In your `.md` file, specify the type of the page with `type: gallery-masonry` or `type: gallery-insta` like this:

``` yaml
---
title: Air is a great hugo theme
type: gallery-masonry
---
Air is a great hugo theme with outstanding features like image gallery from page bundle
```

#### Use as shortcode

Assuming your folder structure would look something like this

``` yaml
content/
└── pages/
    └── my-page/                # Page Bundle
        ├── index.md            # Page content
        ├── featured-image.jpg  # Image Resource used as gallery image 1
        ├── card.jpg            # Image Resource used as gallery image 2 AND as card featured image
        ├── photo1.jpg          # Image Resource used as gallery image 3
        ├── photo2.jpg          # Image Resource used as gallery image 4
        └── photo3.jpg          # Image Resource used as gallery image 5
```

In your `.md` file, add this block to display your instagram image gallery

`{{` `< gallery-masonry page="my-page" >` `}}`

where "my-page" is the page bundle object passed as a variable to the shortcode

Alternatively, use instagram gallery style with

`{{` `< gallery-insta page="my-page" >` `}}`

### Custom Header image

Add one image called `featured-image.jpg` in your page bundle.

#### Use as a featured header image in `single.html`

Automatically loaded as a header image on your page

##### Use the default featured header image

Automatically loaded from the `static/img` folder. - `header-960.jpg` for screens higher than 960px - `header-480.jpg` for screens lower than 960px

### Custom Boostrap Card image

#### Use as featured card image in `list.html`

When listing pages/posts, it displays boostrap cards with a thumbnail image.\
By default it uses the card image from `static/img/card.jpg` Customize the card image by adding one image called `featured-image.jpg` or `card.jpg` in your page bundle.

### Single-page landing homepage

Add pages to a folder. These page will render as a single-page.

Example with this page bundle:

``` yaml
content/
└── landing-page/
    └── page-1/                 # Page Bundle
        ├── featured-image.jpg  # 
        ├── index.md            # Page 1
    ├── _index.md               # File that calls the landing-page type
    ├── page-2.md               # Page 2
    ├── page-3.md               # Page 3
    ├── page-4.md               # Page 4
    └── page-5.md               # Page 5
```

Edit your `content/landing-page/_index.md` to add `type: landing-page`

``` yaml
---
title: Landing Page
catchline: Awesome One Page Landing Page
type: landing-page
---
```

Add a weight to each page to render them by weight ✨:

``` yaml
---
title: Page 1
weight: 10
---
Content of Page 1
```

## Screenshot

\### Mobile {{< img "img/hugo-air-theme-mobile.jpg" "Screenshot of mobile version" >}}

\### Desktop {{< img "img/hugo-air-theme-desktop.jpg" "Screenshot of mobile version" >}}
