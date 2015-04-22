Install prerequisites for building Jasmine
==========================================

As root/admin:

You need to install bundler:
  gem install bundler

BEFORE you run 'bundle' you must first install the nokogiri prerequisites or you'll get a install failure halfway down.
Follow the recipe described at:
  http://nokogiri.org/tutorials/installing_nokogiri.html

Once you have completed the above, you must run the command:
  bundle
in the jasmine root directory. This should install a metric ton of ruby dung and when nothing fails you're good to go.

Then there's also this:
  gem install thor
and this:
  gem install rocco

Now exit root/admin mode and be a regular user again.



Building Jasmine
----------------

To regenerate the jasmine core files, now run:
  thor jasmine_dev:build_distribution

When you want to know what other build commands are available, run:
  thor jasmine_dev
or
  thor list
