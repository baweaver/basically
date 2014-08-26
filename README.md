# Basically

Basically a Rails Model Object, nothing more.

Testing libraries tend to be slow due to their interactions with databases, and this can be
prevented using stubbing and structs.

This is a test project based on some
experiments that yielded much faster mock objects than factories that
have no need to be updated constantly by hand. Rails objects can already
tell you what their columns and types are, why bother telling it again?

By adding a hook to database migrations and creating generators for
certain data types, we can cut the time for factory creation by about
1000x. More rigorous benchmarks will be added to substantiate this claim
as we round into the first release.

## Warning

Fair warning, this is a thought experiment at this point. I would use
caution in putting it in a production system until which time I remove
this paragraph.

## Installation

Add this line to your application's Gemfile:

    gem 'basically'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install basically

## Usage

TODO: Will update with v0.0.1

## Contributing

1. Fork it ( https://github.com/[my-github-username]/basically/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
