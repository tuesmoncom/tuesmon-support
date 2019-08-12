# Tuesmon-support

[![Kaleidos Project](http://kaleidos.net/static/img/badge.png)](https://github.com/kaleidos "Kaleidos Project")
[![Managed with Tuesmon.com](https://img.shields.io/badge/managed%20with-TUESMON.io-709f14.svg)](https://manage.tuesmon.com/project/tuesmon/ "Managed with Tuesmon.com")
[![Build Status](https://img.shields.io/travis/tuesmoncom/tuesmon-support.svg)](https://travis-ci.org/tuesmoncom/tuesmon-support "Build Status")

User support pages for Tuesmon.


#### Envs

- **Stable** (Production Env): [https://manage.tuesmon.com/support/](https://manage.tuesmon.com/support/)
- **Dev** (Test Env): [https://tuesmoncom.github.io/tuesmon-support/](https://tuesmoncom.github.io/tuesmon-support/)


#### Setup

You need:

 - python 2.7
 - node >= 5.0
 - ruby
 - virtualenvwraper


- Install Lektor
```
mkvirtualenv -p /usr/bin/python2.7 tuesmon-support
pip install -r requirements.txt
```

- SASS (need ruby)
```
gem install sass
export PATH=":$PATH:$(ruby -e "print Gem.user_dir")/bin"
sass -v             # should return something like 'Sass 3.4.11 (Selective Steve)'
```

- Install Webpack
```
cd tuesmon-support/webpack
npm install
```


#### Commands

```lektor server -f webpack```
: Run the dev server.

```lektor build -f webpack```
: Build the web site.

```lektor deploy ghpages```
: [CI Enabled] Deploy in GitHub Pages.

```lektor clean```
: Cleans the entire build folder.


#### Code of Conduct

Help us keep the Tuesmon Community open and inclusive. Please read and follow our [Code of Conduct](https://github.com/tuesmoncom/code-of-conduct/blob/master/CODE_OF_CONDUCT.md).
