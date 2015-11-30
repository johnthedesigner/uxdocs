#How to Update UXDocs

##About UXDocs

This site is a Github-hosted, Jekyll-generated static website at the following address:

    http://johnthedesigner.github.io/uxdocs/

##Clone it!

    git clone https://github.com/johnthedesigner/uxdocs.git
    
##Making Updates

For now, updates to our UX documentation could either be made in a new branch or directly in the `master` branch. In order to deploy your updates, you must make a pull request into the `gh-pages` branch. Once the pull request has been merged the changes will become immediately available on the UXDocs website:

    http://johnthedesigner.github.io/uxdocs/

##Creating a new page

To add a new page of documentation, use the following command in terminal from the root of this repo. Replace "My First UXDocs Page" with an appropriate title for your new page. 

    cd uxdocs
    ruby bin/jekyll-page "My First UXDocs Page" ref
    
In the above example, "ref" is the category for this new page there are several available categories listed in `/_config.yml` including `ref`, `memes`, `haiku` and `bad jokes`.

New categories can be added by adding additional items to the array of categories in `/_config.yml`.

A new page will be created and pre-populated with some appropriate front-matter, but you may also wish to add an order number to specify in which order this page should be displayed within its category.

Your newly created file should look like this:

    ---
    layout: page
    title: "My New Page"
    category: ref
    date: 2015-06-05 12:00:00
    ---
    
Edit it to look something like this:

    ---
    layout: page
    title: "My New Page"
    category: ref
    date: 2015-06-05 12:00:00
    order: 1
    ---