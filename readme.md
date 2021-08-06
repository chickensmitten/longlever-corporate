#Run Server

To run server, type `bundle exec jekyll serve` in CLI

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

