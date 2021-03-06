# Hey, you should probably just use Heroku.

## Capinatra

Helpers for deploying Sinatra apps on Passenger.

## Usage

In your Sinatra app's project root, run:

    $ capinatra

This will generate a Capfile for you. After filling
in the appropriate details, you can generate an apache
virtual host by running:

    $ cap capinatra:vhost

You can also choose to copy the Rack configuration
template to your directory by running:

    $ cap capinatra:copy_config

This is useful if you want to override the defaults we've
set for you.  This copied file will take precedence over
the Capinatra-supplied template.

Then it's the usual drill:

    $ cap deploy:setup
    $ cap deploy

(c) Copyright 2008 Pat Nakajima. All Rights Reserved. 