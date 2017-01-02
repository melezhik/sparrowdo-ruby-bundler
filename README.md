# SYNOPSIS

Sparrowdo module to manage Ruby gems via Ruby bundler.

# Travis build status

[![Build Status](https://travis-ci.org/melezhik/sparrowdo-ruby-bundler.svg)](https://travis-ci.org/melezhik/sparrowdo-ruby-bundler)


# INSTALL

    $ panda install Sparrowdo::Ruby::Bundler

# USAGE

Right now all this module does is install RubyGem dependencies straight away from Gemfile.
Probably eventually I will add some other possibilities.


    $ cat sparrowfile

    # runs bundle install for a Gemfile located at the directory:
    ruby_bundler %(
      gemfile_dir => '/path/to/directory/with/gemfile',
    );


# Parameters


## gemfile_dir

Path to the directory with Gemfile. Obligatory, no default value.


## path

The location to install the specified gems to. Optional, no default value.


## verbose

Sets verbose mode. Default value is 0 ( quite mode ). Optional.

## user

Runs bundler for specified user. It's handy when doing user's `bundle install`, not system wide.

# Author

Alexey Melezhik


# See also

[Ruby bundler](http://bundler.io)
