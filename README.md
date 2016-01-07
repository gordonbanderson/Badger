#Badger
##Introduction
This Ruby script adds or replaced badges for a Composer based PHP project hosted
on GitHub that is built with Travis and has code coverage.  It adds badges for
the following:

Travis:
* Build success or fail

Scrutinizer:
* Build success or fail
* Code coverage percentage
* Score, a measure of how clean your code is.

Codecov
* Code coverage percentage, this has a link to a report of your project
showing which lines of code were actually executed during the tests.
* Graph of code coverage for the last 20 commits

Packagist:
* Stable and unstable versions
* Number of downloads
* License
* Downloads this month
* Downloads today

#Install
* Install Ruby if it is not already available on your system
* Copy `badger` to somewhere on the system path, e.g. `~/bin'

#Usage
* Ensure that your code is backed up in Git.
* `cd /path/to/module'
* `badger`

That's it.  This will automatically take account of the current branch, name of
composer project (from composer.json), GitHub username and project (from
`.git/config`)

When a new branch is created simply run the script again.  It will replace
badges from the previous branch.
