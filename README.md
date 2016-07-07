# Automated testing 
* Contributors: bobbingwide
* Donate link: http://www.oik-plugins.com/oik/oik-donate/
* Tags: PHPUnit, automated, testing
* Requires at least: 4.0
* Tested up to: 4.1-beta1
* Stable tag: 4.0
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

The purpose of this plugin is simply to allow WP-a2z to be run against it.
Developers can then view the tests and navigate through them as if they were a real plugin.

To get WP-A2z to work locally I simply created a symbolic link
from the latest SVN version to a plugin directory

cd wp-content/plugins
mklink /J wordpress-develop-tests svn\wordpress-develop\tests


## Installation 

* Not intended for installation into a WordPress environment.
* The zip file is built from the tests folder of the wordpress-develop SVN repository.



## Frequently Asked Questions 
# What does this plugin do? 
Nothing as a plugin. You have to invoke the tests using PHPUnit

# What would happen if I did actually run this? 
Nothing.

If you happened to configure your database the same as your live site then you could destroy your live site.
But the plugin file doesn't contain any code so this is very unlikely.

# Can I run the tests from my WordPress site? 
I'm sure you could try to do this but I can't see why you'd want to.


# How does this help me to develop WordPress tests? 
In the same way that WP-a2z.org helps you to develop WordPress code
this provides you with a dynamic reference of current tests.

# Have you actually tried using this? 
No, I'm in the process of building the API reference as I write this readme.txt


## Screenshots 
1. None

## Upgrade Notice 
# 4.1-beta1 
Built from an update performed on 20 Nov 2014

# 4.0 
* New build from revision 30427 - WordPress 4.0.?

## Changelog 
# 4.1-beta1 
* Changed: See SVN repository for the change log of the tests


# 4.0 
* Added: New for develop.wp-a2z.org

## Further reading 

Extract the latest version of WordPress developer from

https://develop.svn.wordpress.org/trunk/
this will also extract the latest version of the source.


Read about PHPUnit


[bw_link phpunit.de/manual/4.3/en/index.html]

Read about Automated testing on make.wordpress.org

[bw_link make.wordpress.org/core/handbook/automated-testing]

