#Run Server Locally

To run server, type `bundle exec jekyll serve --config _config.yml,_config_dev.yml` in CLI

This ensures that the command line runs the dev config.yml file rather than the production config.yml file

----------------------------------------------------

### Installation problems

When installing, there is an issue where Ruby 3 doesn't have webrick. It gives an error that says:

`bundler: failed to load command: jekyll (/Users/usr/.rbenv/versions/3.0.0/bin/jekyll)
/Users/usr/.rbenv/versions/3.0.0/lib/ruby/gems/3.0.0/gems/jekyll-4.2.0/lib/jekyll/commands/serve/servlet.rb:3:in 'require': cannot load such file -- webrick (LoadError)`

It basically means, it is unable to find webrick. So we need to install it. It can be installed with the command below:

`bundle add webrick`

[Link](https://talk.jekyllrb.com/t/load-error-cannot-load-such-file-webrick/5417/6)

----------------------------------------------------

### First time initiating

`Markdown processor: "redcarpet" is not a valid Markdown processor.
                    Available processors are: kramdown`

Jekyll 4.0 onwards no longer support redcarpet. Have to change to kramdown.

[Link](https://github.com/jekyll/jekyll/issues/7838)

----------------------------------------------------

### JS, CSS and Images not loading

Change the base URL and URL in `_config.yml` like below:

`url: "https://chickensmitten.github.io"
baseurl: "/longlever-corporate"`

Then change the assets to include the base URL and URL like below:

`{{ site.url }}{{ site.baseurl }}/css/framework.css`



------------------------------------------------------

All CSS changes is in Style.css, it has been commented with "heydavid" for clarity

Blue: #5963a7
D. Blue: #405a97
Green: #69a193
Orange: #e1a76b
Orange 20% lighter: #ffda9e

google "colour picker" to choose color













