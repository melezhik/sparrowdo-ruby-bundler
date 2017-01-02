# SYNOPSIS

Manages Ruby gems via Ruby bundler.

# INSTALL

    $ panda install Sparrowdo::Ruby::Bundler

# USAGE

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

Sets verbosity. Default value is 0 ( no verbosity ). Optional.

## user

Runs bundler for specified user. It's handy when doing user's `bundle install`, not system wide.

## http_proxy

Sets http proxy server. If you are under firewall and http traffic is restricted to use http proxy,
use this parameter to set proxy server.


# Author

Alexey Melezhik


# See also

[Ruby bundler](http://bundler.io)
