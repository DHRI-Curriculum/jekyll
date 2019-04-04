
# Installation

## Windows

Note that Jekyll does not officully support Windows. But it still works.

1. Download the latest version of (RubyInstaller for Windows)[https://rubyinstaller.org/downloads/]. This should be the first item under the heading "WITH DEVKIT."
2. Run the executable installer. Use default options.
3. At installation completion, leave the box checked that allows installation to the command line.
4. When closing the installer, a command line should appear with a menu prompt. Type `1` and press `Enter`.
5. Once the menu appears again, press `Enter` to close it.
6. Click the Start menu or press the Windows button on your keyboard (the button near Control).
7. Type `cmd` and press `Enter`.
8. At the command line, type these commands:

```
gem install jekyll
gem install bundler
```

At this point, Jekyll should be installed and available. You can type `jekyll --version` to confirm that it's available to you.

## Mac OS

### First things first: Homebrew

To install Jekyll, you'll first need Ruby. And to install Ruby, you'll first need Homebrew.

Open your terminal by clicking the magnifying glass in the top right of your desktop and typing `terminal` in the bar that appears. Terminal should be the first application that appears.

Enter the following:

```sh
xcode-select --install
```

You may need to agree to a terms and conditions window that appears.

After the installation above completes, enter the following to install Homebrew. (Make sure you don't omit the beginning or end of this command.)

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Time to install Ruby

You should now be able to run the following command in your command line in order to install Ruby:

```sh
brew install ruby
```

Once the install finishes, you can test that the ruby install worked by running the following command:

```sh
which ruby
```

The response should be the path to the ruby installation on your computer. If you run into any troubles in the last steps above, try adding the path to your shell configuration by running:

```sh
export PATH=/usr/local/opt/ruby/bin:$PATH
```

If you have any trouble with the install beyond what is covered here, the Jekyll website provides some great [Troubleshooting advice](https://jekyllrb.com/docs/troubleshooting/)

### Finally, Jekyll!

Now we are ready to install Jekyll, which is easily accomplished by running the following command in your terminal:

```sh
gem install bundler jekyll
```

That should be it! We're ready to go. If you want to double check whether Jekyll is installed, run the following command:

```sh
jekyll -v
```

It should provide you with the version number of the local Jekyll installation.
