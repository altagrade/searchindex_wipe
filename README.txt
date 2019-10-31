Description
-----------

This module cleans up search index built by search module. It is helpful
while deploying large sites whose search index becomes massive. The
reindex button does not clear the search index but rather gradually
replaces existing search data with new data as items are reindexed.


Requirements
------------

Needs the core Search module to be enabled on the site.

Installation
------------

* Download the module from https://github.com/backdrop-contrib/searchindex_wipe
* Enable it via website's user interface or with `drush en searchindex_wipe`
  command on CLI.


Configuration
-------------

* To clear the search index, go to Administration » Configuration » Search and
  metadata » Search settings. Hit on Wipe Index button.

FAQ
---

Q: Why should I use this module?

A: The search index can become massive on large sites, making it difficult
   to transfer the site to another server. Examples include migrating ISPs
   or just creating a test site. Yes, we know it would be better to not delete
   the entire search index, but its sheer size sometimes forces the need.


Q: I wiped my search index, How do I rebuilt it?

A: It is similar to Invalidate Search Index button, i.e. you need to run cron on the site to
   rebuilt the index.


Credits
-------

* Created for Drupal and maintained by Sagar Ramgade (http://drupal.org/user/399718)
  and Nitesh Pawar (http://drupal.org/user/1069334)
* Ported to Backdrop and currently maintained by Alan Mels (https://github.com/alanmels).
