w3lists
=======

Scrape http://lists.w3.org/ to create a threaded tree.

* Can include multiple periods.
* Can follow in-reply-to even when they are in different URLs.

## EXAMPLE:

    w3lists -f text http://lists.w3.org/Archives/Public/www-style/{2013Oct,2013Nov,2013Dec,2014Jan,2014Feb,2014Mar,2014Apr}/
