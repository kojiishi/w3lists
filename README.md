w3lists
=======

Scrape http://lists.w3.org/ to create a threaded-tree.

* Can build one thread-tree from multiple periods/pages
* Can follow in-reply-to even when they are not in the scraping targets.

## Prerequisite

* Python 2.7
* `sudo pip install requests`

## EXAMPLE

    w3lists -f text http://lists.w3.org/Archives/Public/www-style/{2013Oct,2013Nov,2013Dec,2014Jan,2014Feb,2014Mar,2014Apr}/

This command:

1. Scrapes all e-mails from 7 pages; 2013Oct to 2014Apr
2. Finds e-mails of "text" in its subject
3. Collects original e-mails when collected e-mails are replies
4. Prints thread-tree

The output looks like this:

```
[subject]
  [URL] [date] [author]
  [URL] [date] [author]
  ...
```
You can find an example of output [here](https://raw.githubusercontent.com/kojiishi/w3lists/master/text-2013-10.txt).
