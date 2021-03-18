# stsci-exocoffee
This repository stores the website for the Exocoffee Journal Club at STScI.

## How to edit website content

Editing the website is _extremely_ simple. Simply edit the `index.md` file --- that file contains all the info that's displayed in the website. 
If you are a moderator, simply add papers and presenters in the respective columns --- and that's it! Let @nespinoza know so he can update the website.

## How to update the website at www.stsci.edu/~exocoffee

First, you need to install `ruby`, `bundler` and `jekyll`; see, e.g., [this github tutorial](https://docs.github.com/en/enterprise-server@3.0/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll). An even easier way of accomplishing this is with `conda` --- simply do `conda install -c conda-forge rb-jekyll`. Once that is set, you need to update/compile this site locally following these steps:

1. Clone this repository.
2. Do `bundle update`. This will install/update all packages necesary to compile this site.
3. Do `bundle exec jekyll build`. This will create a `_site` directory. You can check the website locally with that doing `bundle exec jekyll build serve` and opening http://localhost:4000.
4. Copy the contents of the `_site` directory to `/grp/webpages/exocoffee`. 
5. That's it! You should see the site updated in https://www.stsci.edu/~exocoffee.
