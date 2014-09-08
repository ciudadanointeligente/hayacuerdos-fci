hayacuerdo
==========

Site that aims to provide graphical evidence of conflicts.

## Installation

- Install Jekyll: `gem install jekyll`
- [Fork this repository](https://github.com/ciudadanointeligente/hayacuerdos-fci/fork) *Optional*
- Clone it: `git clone https://github.com/ciudadanointeligente/hayacuerdos-fci`
- Run the jekyll server: `jekyll --server`
- If you have problems with baseurl run this: 'jekyll serve --watch --baseurl='

You should have a server up and running locally at <http://localhost:4000>.

## Customization

Next you'll want to change a few things. Most of them can be changed directly in
[_config.yml](https://github.com/ciudadanointeligente/hayacuerdos-fci/blob/gh-pages/_config.yml). That's
where we'll pull your name, Twitter username, and things like that.

There's a few other places that you'll want to change, too:

- [CNAME](https://github.com/ciudadanointeligente/hayacuerdos-fci/blob/gh-pages/CNAME): If you're using
  this on GitHub Pages with a custom domain name, you'll want to change this
  to be the domain you're going to use. All that should be in here is a
  domain name on the first line and nothing else (like: `example.com`).
- [favicon.ico](https://github.com/ciudadanointeligente/hayacuerdos-fci/blob/gh-pages/favicon.ico): This
  is a smaller version of my gravatar for use as the icon in your browser's
  address bar. You should change it to whatever you'd like.
- [apple-touch-icon.png](https://github.com/ciudadanointeligente/hayacuerdos-fci/blob/gh-pages/apple-touch-icon.png):
  Again, this is my gravatar, and it shows up in iOS and various other apps
  that use this file as an "icon" for your site.

## Google docs

- Create a google spreadsheet
- Publish it to the web: file -> publish to the web -> select 'entire document' -> press 'publish'
- The generated hiperlink must be declared in _config.yml in gsheet* (where * is the descriptive name of your comparison)
- Create a new sheet for each comparison, with the name in lowercase. For example: government-oposition
- Each sheet must include the following column headers: 'postura1' , 'postura1_txt_largo' , 'postura2' , 'postura2_txt_largo' , 'class'.
  Following the previous example: 
    postura1 = government position
    postura1_txt_largo = government position detail
    postura2 = oposition position
    postura2_txt_largo = oposition position detail
    class = defines the closeness between positions ('acuerdototal', 'acuerdoparcial', 'noacuerdo)
      acuerdototal = agreement
      acuerdoparcial = partial agreement
      noacuerdo = no agreement
- Download the [example sheet](https://docs.google.com/spreadsheets/d/1V2gqtFl7rvZOv9Hbd4f5_3Z45OsyqVyht7FxE5EtiK8/edit?usp=sharing)

## How to integrate the google spreadsheet to the website

- Create a folder on the root named after your comparison that contains index.html. In this file you must call the folder with the comparator.html
- Inside the _includes folder, you must create a folder that will contain comparisons.
- This must contain at least comparator.html file.
- Inside comparator.html search for the div class="sheet_page" and enter the name of the first sheet (of your spreadsheet) that you want to load.
- Then you must define your public_spreadsheet_url
- Finally inside the 'wanted' tag you must specify each sheet to display. 
- Review hayacuerdo.js in the 'switch' section to define the name of the list-box you want to display.

## Deployment

You should deploy with [GitHub Pages](http://pages.github.com)- it's just
easier.

All you should have to do is rename your repository on GitHub to be
`username.github.com`. Since everything is on the `gh-pages` branch, you
should be able to see your new site at <http://username.github.com>.

### Everything else:

For more information about us, our site [Fundación Ciudadano Inteligente](http://www.ciudadanointeligente.org/).
And if you want help with patches, report bugs or replicate our project check [our repositories](https://github.com/ciudadanointeligente/).