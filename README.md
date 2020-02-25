[![Build Status](https://travis-ci.org/tseemann/perl-biotool.svg?branch=master)](https://travis-ci.org/tseemann/perl-biotool)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Don't judge me](https://img.shields.io/badge/Language-Perl_5-steelblue.svg)

:warning: This software is still in early development

# perl-biotool

Small pure Perl5 libraries for writing command line bioinformatics tools

## Introduction

This is a Github template for my Perl based bioinformatics tools.

* search and replace `perl-biotool` with the name of your repo
* enable TRAVIS-CI for the repo

## Quick Start

```
% perl-biotool --version
perl-biotool 0.1.2

```

## Installation

### Conda
Install [Bioconda](https://bioconda.github.io/user/install.html) then:
```
conda install -c conda-forge -c bioconda -c defaults perl-biotool # COMING SOON
```

### Homebrew
Install [Homebrew](http://brew.sh/) (Mac OS X)
or [Linuxbrew](http://linuxbrew.sh/) (Linux) then:
```
brew install brewsci/bio/perl-biotool # COMING SOON
```

### Source
This will install the latest version direct from Github.
You'll need to add the perl-biotool `bin` directory to your `$PATH`,
and also ensure all the [dependencies](#Dependencies) are installed.
```
cd $HOME
git clone https://github.com/tseemann/perl-biotool.git
$HOME/perl-biotool/bin/perl-biotool --help
```

## Dependencies

* `perl` >= 5.26

## License

perl-biotool is free software, released under the
[GPL 3.0](https://raw.githubusercontent.com/tseemann/perl-biotool/master/LICENSE).

## Issues

Please submit suggestions and bug reports to the
[Issue Tracker](https://github.com/tseemann/perl-biotool/issues)

## Author

[Torsten Seemann](https://twitter.com/torstenseemann)
