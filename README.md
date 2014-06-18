w3lists
=======

This tool updates issues documents used by W3C CSS WG.

An example of such issues documents is [here][css-text-doc].

## Prerequisite

* Python 2.7
* `sudo pip install lxml`

## EXAMPLE

    w3lists -f '\[css-text]' --doc issues-lc-2013.txt --user user:pass

This command:

1. Download mbox files from W3C member server and read them.
2. Finds e-mails of "[css-text]" in its subject.
  * Find the canonical URL of the e-mails.
  * Collects original e-mails when collected e-mails are replies.
3. Group e-mails into issues.
4. Add new issues, or add "Comment" liens to existing issues.

[css-text-doc]: http://dev.w3.org/csswg/css-text/issues-lc-2013.txt
