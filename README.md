# learnlib.github.io

The source code to the [learnlib.de](https://learnlib.de/) website.

## Build instructions

You may either follow the [GitHub Pages documentation](https://docs.github.com/en/pages) to setup your Jekyll environment or follow the following steps which aim at a local development environment.

* Install `ruby` and `ruby-bundler` via your paket manager
  * If your distribution does not provide a separate `ruby-bundler` package you may alternatively install the `rubygems` package and run `gem install bundler`
* In the main repository folder, run `bundle config set --local path '~/.local/share/gem'`
* In the main repository folder, run `bundle install`
* Add `~/.local/share/gem/ruby/3.0.0/bin` (path may change due to your ruby version) to your `$PATH` variable.
* In the main repository folder run `jekyll serve` to build the page locally.
