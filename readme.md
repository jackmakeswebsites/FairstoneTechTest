
# Fairstone technical test

## Issues

### index.html
- The `<nav>` section of the webpage was within the `<head>` - I have moved this into the body section
- The `<nav>` section didn't use correctly formatted links or any container - I have used .navbar-expand and set a container
- The 'about' link was linking to `abou.html` - I have corrected this
- Although ... technically not wrong, the `<style>` section was placed at the bottom of the page before the closing `<body>` tag ... I have chosen to add this to a standalone css file
- Again not really an issue - but I have placed the javascript loading to the end of the page, so the HTML content loads first
- The carousel was referencing three images, the third image (`image4.jpg`) doesn't exist - I have set the third image to load `image3.jpg`
- The carousel wrapper `<div>` referenced the same class twice - I have removed the duplicate class referenced
- Slide 1 & 3 black clashes, so made this lighter text
- Carousel was inconsistent with image heights - I have added some custom css to `custom.css` to make all the images equal in height
- I have created a container for the Modal button
- I have set the footer text to be properly vertically centered within the footer itself

### about.html
- `<nav>` section was in the head again, so copied the nav I created for `index.html` over and set `about.html` as active
- removed the empty `<script>` and `<style>` tags
- Placed `<script>` tags at the end of the `<body>`
- Created a container with top padding so the text isn't obscured by the navbar
- I have created `<p>` tags around each line break of text, to break up the sections - I could have used `<br>` - but this would only add a linebreak
- I have added the `<footer>` to the `about.html` page

### custom.css (originally inline style for `index.html`)
- `.carousel-caption` class had english spelling of `colour` - I changed this to `color` (which is correct for css)
- .title had `fontsize` - I have changed this to `font-size`
- I have commented out the modal section - it appears to be attempting to achieve what bootstrap already achieves off the bat
- To make the modal more like a lightbox, I have added a few custom classes to `custom.css`

### After thoughts
- I have setup the sections `<nav>` / `<main>` / `<footer>`
- I have moved `msh.jpg` into the `img` directory

## Recommendations for `about.html`
Firstly the use of `<nav>` before the `<body>` tag is incorrect, while the navbar is a page header, the `<head>` tag is mainly used for loading stylesheets, setting meta tags, setting the page title (as shown in the tab on the browser) and other scripts to load first on the page

The text section of the page had no container, or any kind of row spacing. Just using a `<div>` tag with a `<p>` tag will not pfovide any styling. What I have done is used bootstrap's in-built container, row and col system to format the text so it shows nicely on the page. Additionally using line breaks on your code editor will not work like on Word - you have to manually create the line spaces by either using a `<br>` tag which will add 1 line - using word as an example - is like reaching the end of you horizonatal space and going onto a new line - using `<p>` tags will ad 1 line of whitespace between each section. Always remember to close your `<p>` tags.

Additionally, within your `<p>` tags you can use `<a>` tags to create clickable links


## What would I recommend going forward?
Well given there's a ... mediocre ... chance that product listings may be made - not necesarrily in an eCommerce setting, and page categories may be required, I would recommend a CMS service like Wordpress. Wordpress has many out of the box templates and visual editors - such as Elementor, WP Bakery (free options) and also some premium themes come with their own built in editors - such as Divi. 

Wordpress makes it easy to create websites and design with a fully visual editor, manage media, manage pages, posts and categories with ease. as well as a 'drag and drop' menu builder.

Also with Wordpress there is an exhaustive list of plugins allowing for endless customisability.

I would recommend using one of the free themes provided on Wordpress (given this is a simple Bootstrap website) and using Elementor (a free visual editor plugin).


