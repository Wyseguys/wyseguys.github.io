# Wyseguys.com

Wyseguys.com is the personal site of Chris Zwemke.  As a web developer by trade and by interest, this site represents the place where Chris can put his best quality work forward.  Sure there is a mild amount of monetized content that gets a few thousand visitors per year, but that is really just used as another set of real world tests.  For example, when I use a new blog engine, can I configure and keep the old traffic from the previous links out in the world?

# Jekyll

This is a Jekyll generated blog.  It is developed on Windows 10 pro, using Visual Studio Code and Windows Subsystem for Linux..

# minima

*Minima is a one-size-fits-all Jekyll theme for writers*. It's Jekyll's default (and first) theme. It's what I got when I ran `jekyll new`.

[Theme preview](https://jekyll.github.io/minima/)

![minima theme preview](/screenshot.png)

## Installation

Follow the instructions at https://jekyllrb.com/docs/ in the quickstart.  Even though I am using Windows 10 Pro, follow the linux instructions because we are doing the WSL.  It works great.

I keep the code in a directory on my C:, that I created a symlink in WSL to.  So when I first start the WSL, my folder is symlinked in the home directory and it is quick and easy to run

sudo bundle exec jekyll serve --incremental

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/jekyll/minima. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `script/bootstrap`.

To test your theme, run `script/server` (or `bundle exec jekyll serve`) and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme and the contents. As you make modifications, your site will regenerate and you should see the changes in the browser after a refresh.

## License

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
