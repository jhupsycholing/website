# caplabjhu.org

Website for Tal Linzen's Computation and Psycholinguistics lab at Johns Hopkins University.


## Updating the site on Webfaction

Clone this repo and make any edits you need, then run `bundle exec jekyll serve` in the main 
directory to create the `_site` directory and debug the site locally. 

#### New to Jekyll?
This site is made with the *static site generator* [Jekyll](https://jekyllrb.com/docs/), which you'll need to have 
installed along with the latest version of [Ruby](https://www.ruby-lang.org/en/documentation/installation/). 
If you're doing a fresh install, make sure to `cd` to this repo directory and run `gem install jekyll bundler`
and then `bundle install` to install all the dependencies and plugins needed before doing `bundle exec jekyll serve`.

#### Going live
Once you are happy with the way the site looks, push the changes to this repo. Then clear 
the contents of `~/webapps/jhu_psycholing_site` on our Webfaction account (`ssh jhpsycholing@web513.webfaction.com`).
Once you have done so, you can copy the contents of the updated static `_site` you just built 
using `scp` by running `scp -r _site/* jhpsycholing@web513.webfaction.com:/home/jhpsycholing/webapps/jhu_comp_psycholing_site`.

Not the most elegant solution, but I haven't yet figured out how to update the site automatically with each new
push on the Github repo. In the meantime this solution should still work just fine. (-Karl 10/2/19)

## Site Components

Parts of the site you are most likely to edit. 

#### Papers
Update publications by adding the BibTeX entry to `_bibliography/In Progress.bib` or `_bibliography/Published.bib`. 

#### News
Add a new news item to `_data/news.csv`.

#### People

Add a new lab member to `_data/people.csv`.


