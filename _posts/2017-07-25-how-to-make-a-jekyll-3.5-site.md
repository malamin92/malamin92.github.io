---
layout: post
---
## What is Jekyll?
[Jekyll](https://jekyllrb.com/) according to their site "...is a simple, blog-aware, static site generator." That sure is a fancy definition but what does it mean? What Jekyll allows you to do is write [markdown](https://guides.github.com/features/mastering-markdown/) files and turn them into static HTML pages. Jekyll is especially awesome because you can actually host your Jekyll content site for free via [Github](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/). I find that Jekyll is great way for developers (or anyone code savvy) to host a simple, static, content site (like a blog or portfolio site).

##  Github Pages
If you do not already know, the [Gitgub Pages](https://pages.github.com/) feature allows you to host static HTML pages on github for free. To get started with this, all you need to do is create a repo with a name in the following format: your_username.github.io. Once you do this, you can put any static html file in there with the name index.html and it will be the home page of you site. For example, my username is moalamin, my github pages link is: "[https://moalamin.github.io](https://moalamin.github.io)".

Once you created a repo on your github with the correct format, you are free to code your static site however you want. Clone the repo and code away! Just remember, the homepage will always be the index.html file at the root of your repo. However, if you do not want to spend too much time coding up your entire site, what you can do is generate a Jekyll site. Due to the way Jekyll works, it will generate an index.html file for you in the root directory, with a preinstalled theme that you can fully customize and add to.

## Installing Jekyll
In order to install Jekyll and have it work with your site, you need to have `Ruby 2.1.0` or higher installed on your computer along with the [bundler gem](http://bundler.io/). You can check which version of `Ruby` you have installed by typing `ruby -v` into your terminal. Once you confirm you have the propper version of Ruby installed, go ahead and install the [bundler gem](http://bundler.io/). If you ever want to check if you have an utility installed and exposed to your Terminal session, you can type `which utility_name`, for example, for bundler I can write `which bundler`. If a path to a directory is displayed, that means the utility is installed at that directory.

Confirm that you have `Ruby` and `bundler` installed. The next step is to install the Jekyll gem. You can do so by typing `gem install jekyll` into your terminal. With jekyll installed, navigate to a directory where you want to create your jekyll project. Create a new Jekyll project by typing `jekyll new name-of-github-pages-repo`. You want to keep the name of the project the same as your github pages repo for consistencies sake. You can `cd` into your repo and there you have it, you have successfully generate your Jekyll project. In the Jekyll project directory, run `jekyll serve` in the terminal and you will be to visit your site at localhost:4000, similar to how you visit a Rails server or Express server. This is how your site will look like when users visit them. By default Jekyll ships with the minima theme, you can change this at will.

## Writing a Blog Entry
You can begin writing blog entries for your site by creating a markdown file in the `_posts` folder. The name  of the markdown has to follow a certain format: *year-month-date-title-of-blog*. Go ahead and write as your desire! You can also find information on [markdown format here](https://guides.github.com/features/mastering-markdown/).

## Getting the Jekyll site on GitHub
Now let's get your new site up on github. This is pretty standard stuff, just initialize your Jekyll project folder with `git init`. Do your initial `git add` and `git commit -m 'first commit message'`. Go ahead and get the link to the repo you created earlier and do `git remote set origin link-to-repo` . The last step is to push your project folder with `git push origin master` (or a branch if you created one).

You did it! Your site should be up in a couple of minutes with the front page showing whatever blog entries you have written so far. Go ahead and give yourself a pat on the back.

## Summary and Additional Resources
This blog went over the basics of github pages and how to get a [Jekyll](https://jekyllrb.com/) site on there. You can go ahead and customize your site. I found it a little confusing to customize Jekyll 3.5, [check the docs here](https://github.com/jekyll/minima#customization) for some tips. You can find the `minima` theme installed on your computer by using `bundle show minima` command and then navigating to the directory shown. You can customize any file by copying it over to your project folder, but remember to keep the folder structure and file name the same as it is in your `minima` theme structure.

A quick way to customize your site is by looking in your `_config.yml` file that was generate by Jekyll and filling in the information it asks for.

Happy coding!
