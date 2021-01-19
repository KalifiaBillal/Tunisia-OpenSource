# [opensourcedesign.net](https://opensourcedesign.net)

Website of the Open Source Design community, hosted on GitHub Pages.

[![Backers on Open Collective](https://opencollective.com/opensourcedesign/backers/badge.svg)](#backers) [![Sponsors on Open Collective](https://opencollective.com/opensourcedesign/sponsors/badge.svg)](#sponsors) [![Twitter Follow](https://img.shields.io/twitter/follow/opensrcdesign?style=social)](https://twitter.com/opensrcdesign)

### Installing

This step requires having a `ruby` development environment and `git` installed
and configured to connect to GitHub with SSH.

- [Installing Ruby][installing-ruby]
- [Using GitHub with SSH][github-ssh]

1. Install Jekyll using and other Ruby gems

```sh
sudo gem install bundler
```

2. Fork and clone the main website repository

```sh
git clone --single-branch --branch master https://github.com/opensourcedesign/opensourcedesign.github.io.git
cd opensourcedesign.github.io/
bundle install
```

3. Run our installer script

This will pull down all of the repositories (jobs, events, etc...) and put them
in there proper place to build our website locally.

```sh
./scripts/install.sh
```

*Note: you need to be a member of our [GitHub organization][osd-org].*

4. Build the static site & watch for files

```sh
bundler exec jekyll serve --watch --config _config.yml,_config-dev.yml
```

## 📜 License

**🔀 You can use & modify everything as long as you credit [Open Source Design](https://opensourcedesign.net) and use the same license for your resulting work.** [Code license is AGPLv3](https://www.gnu.org/licenses/agpl-3.0.en.html) and content is [Creative Commons Attribution-ShareAlike](https://creativecommons.org/licenses/by-sa/4.0/).
