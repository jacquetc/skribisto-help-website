# Skribisto Help Website

## For developers

### Preview your changes

After having modified the project on the "develop" branch, follow these instructions:

(Taken from [here](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll))

```bash
cd ~
sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
gem install jekyll bundler

cd ~/Devel/skribisto-help-website
bundle install
```

Then,
```bash
bundle exec jekyll serve
```

In your browser go to (http://localhost:4000/)[http://localhost:4000/]

After this last command, whenever you make a change made in the project, the generated website will reflect it.
