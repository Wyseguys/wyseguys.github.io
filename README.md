# Wyseguys.com

Wyseguys.com is the personal site of Chris Zwemke.  As a web developer by trade and by interest, this site represents the place where Chris can put his best quality work forward.  Sure there is a mild amount of monetized content that gets a few thousand visitors per year, but that is really just used as another set of real world tests.  For example, when I use a new blog engine, can I configure and keep the old traffic from the previous links out in the world?

# Jekyll

This is a Jekyll generated blog.  It is developed on Linux Mint 21.3, using Visual Studio Code and Docker.

# minima

*Minima is a one-size-fits-all Jekyll theme for writers*. It's Jekyll's default (and first) theme. It's what I got when I ran `jekyll new`.

[Theme preview](https://jekyll.github.io/minima/)

![minima theme preview](/screenshot.png)

## Installation

Follow the instructions at https://jekyllrb.com/docs/ in the quickstart.  Even though I am using Windows 10 Pro, follow the linux instructions because we are doing the WSL.  It works great.

I keep the code in a directory home, there is then a DockerFile that will start up an environment.

I copied this setup from https://gist.github.com/BillRaymond/db761d6b53dc4a237b095819d33c7332

0. Local Dev:  git, VS Code (extensions Docker & Dev Containers), Docker Desktop.
1. Clone this repo and open the directory in VS Code
2. ctrl + p, use the "Rebuild Container" command in VS Code
...
3. VS Code will bounce and show you are running the same code in a container.
4. bundle exec jekyll serve --incremental

The last command might prompt you to do the bundle gem install or whatever if you haven't done it in that container before.  No biggy.


## Development

Good luck!

To test your theme, run ` bundle exec jekyll serve --incremental` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme and the contents. As you make modifications, your site will regenerate and you should see the changes in the browser after a refresh.

