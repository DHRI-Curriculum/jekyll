# Getting Started

Now we are ready to get our first site set up and running. In order to do so, we need to create a new site. You can create a site inside an already existing folder but in the following, we'll set up a clean site using Jekyll's own generator.

## Decide Location

First, you need to decide where your site should live locally. In order to navigate to the Desktop folder of your user account, run this command in your command line:

```sh
cd ~/Desktop
```

_In our example, we'll put the site on your computer's desktop but you may want to navigate to a different directory. You can do this by using `cd` as you may remember from our [command line workshop](http://www.github.com/DHRI-Curriculum/command-line)._

We will create a new Jekyll site on the desktop by writing:

```sh
jekyll new my-site
```

This command may take some time to run, so take a break—stand up and stretch your arms—while it runs. Once it is done, your command line should have an output that looks something like this:

```sh
Running bundle install in ~/Desktop/my-site... 
  <span style="color: green;">Bundler:</span> Fetching gem metadata from https://rubygems.org/...........
  <span style="color: green;">Bundler:</span> Fetching gem metadata from https://rubygems.org/.
  <span style="color: green;">Bundler:</span> Resolving dependencies...
  <span style="color: green;">Bundler:</span> Fetching public_suffix 3.0.3
  <span style="color: green;">Bundler:</span> Installing public_suffix 3.0.3
  <span style="color: green;">Bundler:</span> Fetching addressable 2.6.0
  <span style="color: green;">Bundler:</span> Installing addressable 2.6.0
  <span style="color: green;">Bundler:</span> Using bundler 2.0.1
  <span style="color: green;">Bundler:</span> Using colorator 1.1.0
  <span style="color: green;">Bundler:</span> Fetching concurrent-ruby 1.1.5
  <span style="color: green;">Bundler:</span> Installing concurrent-ruby 1.1.5
  <span style="color: green;">Bundler:</span> Fetching eventmachine 1.2.7
  <span style="color: green;">Bundler:</span> Installing eventmachine 1.2.7 with native extensions
  <span style="color: green;">Bundler:</span> Using http_parser.rb 0.6.0
  <span style="color: green;">Bundler:</span> Using em-websocket 0.5.1
  <span style="color: green;">Bundler:</span> Fetching ffi 1.10.0
  <span style="color: green;">Bundler:</span> Installing ffi 1.10.0 with native extensions
  <span style="color: green;">Bundler:</span> Using forwardable-extended 2.6.0
  <span style="color: green;">Bundler:</span> Using i18n 0.9.5
  <span style="color: green;">Bundler:</span> Using rb-fsevent 0.10.3
  <span style="color: green;">Bundler:</span> Fetching rb-inotify 0.10.0
  <span style="color: green;">Bundler:</span> Installing rb-inotify 0.10.0
  <span style="color: green;">Bundler:</span> Using sass-listen 4.0.0
  <span style="color: green;">Bundler:</span> Fetching sass 3.7.4
  <span style="color: green;">Bundler:</span> Installing sass 3.7.4
  <span style="color: green;">Bundler:</span> Using jekyll-sass-converter 1.5.2
  <span style="color: green;">Bundler:</span> Using ruby_dep 1.5.0
  <span style="color: green;">Bundler:</span> Using listen 3.1.5
  <span style="color: green;">Bundler:</span> Fetching jekyll-watch 2.2.1
  <span style="color: green;">Bundler:</span> Installing jekyll-watch 2.2.1
  <span style="color: green;">Bundler:</span> Fetching kramdown 1.17.0
  <span style="color: green;">Bundler:</span> Installing kramdown 1.17.0
  <span style="color: green;">Bundler:</span> Fetching liquid 4.0.3
  <span style="color: green;">Bundler:</span> Installing liquid 4.0.3
  <span style="color: green;">Bundler:</span> Using mercenary 0.3.6
  <span style="color: green;">Bundler:</span> Fetching pathutil 0.16.2
  <span style="color: green;">Bundler:</span> Installing pathutil 0.16.2
  <span style="color: green;">Bundler:</span> Fetching rouge 3.3.0
  <span style="color: green;">Bundler:</span> Installing rouge 3.3.0
  <span style="color: green;">Bundler:</span> Fetching safe_yaml 1.0.5
  <span style="color: green;">Bundler:</span> Installing safe_yaml 1.0.5
  <span style="color: green;">Bundler:</span> Using jekyll 3.8.5
  <span style="color: green;">Bundler:</span> Fetching jekyll-feed 0.12.1
  <span style="color: green;">Bundler:</span> Installing jekyll-feed 0.12.1
  <span style="color: green;">Bundler:</span> Fetching jekyll-seo-tag 2.6.0
  <span style="color: green;">Bundler:</span> Installing jekyll-seo-tag 2.6.0
  <span style="color: green;">Bundler:</span> Fetching minima 2.5.0
  <span style="color: green;">Bundler:</span> Installing minima 2.5.0
  <span style="color: green;">Bundler:</span> Bundle complete! 4 Gemfile dependencies, 29 gems now installed.
  <span style="color: green;">Bundler:</span> Use `bundle info [gemname]` to see where a bundled gem is installed.
  <span style="color: green;">Bundler:</span> Post-install message from sass:
  <span style="color: green;">Bundler:</span> 
  <span style="color: green;">Bundler:</span> Ruby Sass has reached end-of-life and should no longer be used.
  <span style="color: green;">Bundler:</span> 
  <span style="color: green;">Bundler:</span> * If you use Sass as a command-line tool, we recommend using Dart Sass, the new
  <span style="color: green;">Bundler:</span> primary implementation: https://sass-lang.com/install
  <span style="color: green;">Bundler:</span> 
  <span style="color: green;">Bundler:</span> * If you use Sass as a plug-in for a Ruby web framework, we recommend using the
  <span style="color: green;">Bundler:</span> sassc gem: https://github.com/sass/sassc-ruby#readme
  <span style="color: green;">Bundler:</span> 
  <span style="color: green;">Bundler:</span> * For more details, please refer to the Sass blog:
  <span style="color: green;">Bundler:</span> https://sass-lang.com/blog/posts/7828841The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
New jekyll site installed in ~/Desktop/my-site. 
```
