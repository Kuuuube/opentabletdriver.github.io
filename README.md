# opentabletdriver.github.io
The next version of OpenTabletDriver.Web

# Local Development

## Requirements

- `rubygems`

## Steps

```bash
$ gem install jekyll bundler
$ cd <website root> # (currently git root)
$ git submodule init # submodules contain plugin data
$ git submodule update
$ bundle install
$ bundle exec jekyll serve --livereload
```

# FAQ

## How do I add an wiki entry?

Add or edit the appropriate markdown file in the appropriate `_wiki/` folder.

## I can't find the "index" page for a page! (e.g. site/Wiki)

Single-path URL's are permalinked to files in `_sections`

## How do I update the rouge highlighter style?

`bundle exec rougify style > assets/rougehl.css`

## How can I check if I have internal links that don't use the `{% link %}` paradigm?

```bash
cd <website root>
grep -R --exclude-dir vendor --include="*.md" '](' | grep -v '](#' | grep -v ']({%' | grep -v '](http' | grep -v '](//'`
```

## How are the Wiki ToC's generated?

With [allejo/jekyll-toc](https://github.com/allejo/jekyll-toc). We are using 1.2.0.

# Contributors to old OpenTabletDriver.Web

[Link](https://github.com/OpenTabletDriver/OpenTabletDriver.Web/graphs/contributors)

As this site is ported directly from the old repository to Jekyll, the site may contain
code, assets, information or other contributions by:

[@InfinityGhost](https://github.com/InfinityGhost)\\
[@jamesbt365](https://github.com/jamesbt365)\\
[@gonX](https://github.com/gonX)\\
[@vedxyz](https://github.com/vedxyz)\\
[@Hypfer](https://github.com/Hypfer)\\
[@TakanashiDavi](https://github.com/TakanashiDavi)\\
[@Sublimelime](https://github.com/Sublimelime)\\
[@nerd](https://github.com/nerd)\\
[@FlafyDev](https://github.com/FlafyDev)\\
[@DanisDGK](https://github.com/DanisDGK)\\
[@Zyfarok](https://github.com/Zyfarok)\\
[@X9VoiD](https://github.com/X9VoiD)\\
[@MicrochipQ](https://github.com/MicrochipQ)\\
[@vgf89](https://github.com/vgf89)
