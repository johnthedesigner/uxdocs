#How to Update UXDocs

Clone it!

    git clone https://github.com/johnthedesigner/uxdocs.git

##Creating a new page

To add a new page of documentation, use the following command in terminal from the root of this repo. Replace "My First UXDocs Page" with an appropriate title for your new page. 

    cd uxdocs
    ruby bin/jekyll-page "My First UXDocs Page" ref
    
In the above example, "ref" is the category for this new page there are several available categories listed in `/config.yml` including `ref`, `memes`, `haiku` and `bad jokes`.

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