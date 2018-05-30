# What Is a Static Site?

## What's Old Is New Again

In the beginning, there was HTML. Web pages were documents that connected to other documents, and were created by hand-writing HTML.

In the 2000s, a broad trend toward dynamic websites began. Rather than a collection of documents, these websites consisted of template documents backed up by a database. When a user requested a page, the appropriate template would be chosen, the database would be consulted, and the page would be built on the fly and served to the user. WordPress is a well-known example of this dynamic model, but other content management systems such as Drupal as well as proprietary services such as Squarespace and Twitter also use a database-backed dynamic model.

In the mid-2010s, a new paradigm for website creation, the static site generator, began seeing widespread use. Rather than build individual pages at the moment they are requested by the user, these sites take folders of content, often in markdown, and use templates to generate a complete website. The output of this process is then hosted as static HTML files. Static sites are cheaper to host, expose a smaller surface area to hackers, and tend to have more comprehensible internals than comparable dynamic sites. Though static sites are a favorite of technical bloggers, companies like MailChimp and Vox Media have begun to use them to host their primary websites.

## Advantages and Disadvantages

Advantages of static sites:

- Load faster and are cheaper to host.
- Difficult to hack.
- More comprehensible internals.
- Easy to put under version control.
- Can be hosted on any computer/server/host configuration.
- Are often free to host on sites like GitHub, Netlify, or GitLab.
- Require no updates and are less likely to break over time.

Disadvantages of static sites:

- Features dependent on user input, such as comments or "Most popular" widgets, are not possible or require workarounds.
- Non-technical users have a more difficult time contributing content—no WordPress-style admin panel.
- Can be slow to build a large or very large site.

