# sbs
Static Blogging System

sbs is a POSIX compliant static blog generator that generates an HTML blog, an RSS feed,
and a rolling blog page from Markdown.

## Installation

First, make sure [Pandoc](https://pandoc.org/) is installed on your system.

In order to use sbs the `<!-- SB -->` (start blog) tag needs to be added
to your RSS, home page, and rolling blog pages in order to enable those
features. You can use my website repository as an example [here](https://git.sr.ht/~bpv/website)
or my actual website [here](https://brycevandegrift.xyz).

Change all the variables in the beginning of the script according to your
own website specifications as well as create the:
- Website directory
- Blog Directory
- RSS file
- Rolling blog page in blog directory
- Drafts directory
- Home page (index.html)
- CSS stylesheet
- Website icon

You can also set your `EDITOR` variable to use your preferred text editor,
otherwise vi is used by default.

sbs can also be used on a directory by directory basis, just change the
`website_dir` variable to `$(pwd)`.

## Usage

```
sbs new		# Create a new blog post
sbs edit	# Quickly edit existing draft
sbs publish	# Publish a draft and turn it into a webpage
sbs rename	# Rename a draft
sbs delete	# Delete a draft
sbs help	# Show quick help
sbs version	# Show version
```

## Bugs

Please report any bugs or errors to [bryce@brycevandegrift.xyz](mailto://bryce@brycevandegrift.xyz).

## Contributions

Parts of this program were used from [Luke Smith's blog generation script](https://github.com/LukeSmithxyz/lb).

## Notice

In the future I plan to expand on this script in order to add more features
as well as to make it more portable and easier to use.
