w3lists
=======

Scrape http://lists.w3.org/ to create a threaded tree.

* Can include multiple periods.
* Can follow in-reply-to even when the e-mails it replied to is not in the scraping targets.

## Prerequisite

* Python 2.7
* `pip install requests` (Mac may need `sudo pip install requests`)

## EXAMPLE

    w3lists -f text http://lists.w3.org/Archives/Public/www-style/{2013Oct,2013Nov,2013Dec,2014Jan,2014Feb,2014Mar,2014Apr}/

This command:

1. Scrapes all e-mails from 7 pages; 2013Oct to 2014Apr
2. Find e-mails of "text" in its subject
3. Collect original e-mails when collected e-mails are replies
4. Print thread-tree

The output looks like this:

```
[subject]
  [URL] [date] [author]
  [URL] [date] [author]
  ...
```
