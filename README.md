# PATRIC Documentation Repo

This repository is for manage PATRIC static contents such as Website Tutorial, CLI Tutorial, User Guides, and PATRIC eNews. 
See [here](./Setup.md) for configuration.

## How to add an entry
1. Create a folder. If you don't have image associated, then you can ommit the images folder.
```
mkdir -p tutorial/excel_formatting/images/
```

2. Make a markdown or ReST (ReStructuredText) format file

3. Place images under `./images` sub folder

4. Add a link in the category index file (e.g. `tutorial/index.rst`)

5. build html
```
$ make html
```

## How to add a News entry
In order to generate feed RSS, you need to write the news entries in rst format.
Check a sample entry [here](https://github.com/PATRIC3/p3_docs/blob/master/docroot/news/20170930-patric-september-2017-data-release.rst)

1. Follow the instruction for creating a file & linking
2. For news entries, you need to add a code block like below,
```
.. feed-entry::
   :date: 2017-09-30

   Add description (a line or two) regarding the news item here. This will show up in the home page.

.. cut::
```

3. When you build html, `news.rss` will be updated.

## Resources
1. Markdown [cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

2. ReST [quick reference](http://docutils.sourceforge.net/docs/user/rst/quickref.html)
