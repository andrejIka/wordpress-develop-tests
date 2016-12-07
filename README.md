# wordpress-develop-tests 
![banner](https://raw.githubusercontent.com/bobbingwide/wordpress-develop-tests/master/assets/wordpress-develop-tests-banner-772x250.jpg)
* Contributors: bobbingwide
* Donate link: http://www.oik-plugins.com/oik/oik-donate/
* Tags: PHPUnit, automated, testing
* Requires at least: 4.7
* Tested up to: 4.7
* Stable tag: 4.7
* License: GPLv2 or later
* License URI: http://www.gnu.org/licenses/gpl-2.0.html
* Text Domain: default
* Domain Path: /languages/

## Description 
Automated testing of WordPress involves running test cases where manual intervention is not required to run each one.

* WordPress is a complicated system.
* There aren't as many tests as you might have hoped.
* But the team are working on it.
* Each new TRAC could/should be backed up by a new test.

The purpose of this plugin is twofold:

1. To allow the WP-a2z dynamic API reference parser to be run against the PHPUnit tests for WordPress. Developers can then view the tests and navigate through them as if they were a real plugin.
2. To provide the framework functionality for in situ PHPUnit testing of plugins and themes using oik-batch.



## Installation 

* Only intended for installation into a WordPress environment where you'll be running your own PHPUnit tests

* The zip file is built from the tests folder of the wordpress-develop SVN repository.
(  http://develop.svn.wordpress.org/branches/4.7 )



## Frequently Asked Questions 
# What does this plugin do? 
Nothing as a plugin. You have to invoke the tests using PHPUnit.
But since we don't provide the phpunit.xml file it won't work.


# What would happen if I did actually run this? 
If you activate the plugin then nothing is expected to happen since it doesn't contain any code.


If you run PHPUnit then quite a lot might happen.
If you had happened to configure your database the same as your live site then you could destroy your live site.


# Can I run the tests from my WordPress site? 
I'm sure you could try to do this but I can't see why you'd want to.


# How does this help me to develop WordPress tests? 

In the same way that WP-a2z.org helps you to develop WordPress code
this provides you with a dynamic reference of current tests.
See [develop.wp-a2z.org](http://develop.wp-a2z.org)

# Have you actually tried using this? 

Yes.


# What's the process for managing this repo? 

* Original method: Nov 2014

To get WP-A2z to work locally I simply created a symbolic link
from the latest SVN version to a plugin directory

cd wp-content/plugins
mklink /J wordpress-develop-tests svn\wordpress-develop\tests

* Recently: August 2016

This is the latest process used to build the API reference.

- Extract http://develop.svn.wordpress.org/trunk to C:\svn\wordpress-develop
- Change directory to a clone of the GitHub repository bobbingwide/wordpress-develop-tests
- Remove the phpunit and qunit directories
- Copy files from the tests folder, phpunit and qunit
- Commit changes, including any deletions
- Push to GitHub
- Pull into the WP-a2z websites plugin directory
- Build the dynamic API reference for the latest level

* Current method: December 2016

- Extract http://develop.svn.wordpress.org/branch/4.7 to C:\svn\wordpress-develop\4.7
- remaining steps as above



## Screenshots 
1. None

## Upgrade Notice 
# 4.7 
Built from http://develop.svn.wordpress.org/branch/4.7 (on 2016/12/07)

# 4.6  
Built from an SVN extract of trunk taken 2016/08/19

# 4.5.3 
Built from an SVN extract of trunk taken 2016/07/07

# 4.1-beta1 
Built from an update performed on 20 Nov 2014

# 4.0 
* New build from revision 30427 - WordPress 4.0.?

## Changelog 
# 4.7 
* Changed: source files updated to branch/4.7
* Changed: updated readme
* Deleted: Unnecessary phpunit/build and phpunit/data files - accidentally checked in for 4.5.3
* Deleted: phpunit/tests/user/wpSetCurrentUserhm.php - not part of WordPress tests

# 4.6 
* Changed: source files updated to latest extract taken on 2016/08/19
* Fixed: Removed unnecessary .idea files

# 4.5.3 
* Changed: source files updated to latest extract taken on 2016/07/07
* Changed: readme should reflect the new build process
* Fixed: Some files were corrupted with local changes 2016/07/09

# 4.1-beta1 
* Changed: See SVN repository for the change log of the tests

# 4.0 
* Added: New for develop.wp-a2z.org

## Further reading 

Extract the latest version of WordPress developer from

https://develop.svn.wordpress.org/trunk/

This will also extract the latest version of the source.


Read about [PHPUnit](https://phpunit.de/manual/5.7/en/index.html)

Read about [Automated testing on make.wordpress.org](https://make.wordpress.org/core/handbook/automated-testing)

