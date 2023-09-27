

Urban
https://github.com/CloudCannon/urban-jekyll-template

Web Agency themed business template for Jekyll. Browse through a live demo. Increase the web presence of your agency with this configurable theme.

Urban was made by CloudCannon, the Cloud CMS for Jekyll.

Find more templates, themes and step-by-step Jekyll tutorials at CloudCannon Academy.

Features

    Contact form
    Pre-built pages
    Pre-styled components
    Blog with pagination
    Post category pages
    Disqus comments for posts
    Staff and author system
    Configurable footer
    Optimised for editing in CloudCannon
    RSS/Atom feed
    SEO tags
    Google Analytics

Setup

    Add your site and author details in _config.yml.
    Add your Google Analytics and Disqus keys to _config.yml.
    Get a workflow going to see your site's output (with CloudCannon or Jekyll locally).

Develop

Urban was built with Jekyll version 3.3.1, but should support newer versions as well.

Install the dependencies with Bundler:

$ bundle install

Run jekyll commands through Bundler to ensure you're using the right versions:

$ bundle exec jekyll serve

Editing

Urban is already optimised for adding, updating and removing pages, staff, advice, company details and footer elements in CloudCannon.
Posts

    Add, update or remove a post in the Posts collection.
    The Staff Author field links to members in the Staff collection.
    Documentation pages are organised in the navigation by category, with URLs based on the path inside the _docs folder.
    Change the defaults when new posts are created in _posts/_defaults.md.

Contact Form

    Preconfigured to work with CloudCannon, but easily changed to another provider (e.g. FormSpree).
    Sends email to the address listed in company details.

Staff

    Reused around the site to save multiple editing locations.
    Add excluded_in_search: true to any documentation page's front matter to exclude that page in the search results.

Footer

    Exposed as a data file to give clients better access.
    Set in the Data / Footer section.

Company details

    Reused around the site to save multiple editing locations.
    Set in the Data / Company section.

