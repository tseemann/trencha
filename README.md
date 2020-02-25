[![Build Status](https://travis-ci.org/tseemann/trencha.svg?branch=master)](https://travis-ci.org/tseemann/trencha)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Don't judge me](https://img.shields.io/badge/Language-Perl_5-steelblue.svg)

:warning: This software is still in early development

# trencha

Normalize VCF depth for Illumina GC bias

## Introduction

Many variant calling pipelines using sequencing depth (the `DP` tag) 
to help remove false positive variants. A common threshold is `DP >= 10`.
The assumption is that all parts of the genome are sequenced
equally, but it is well understood that Illumina sequencing drops off
in extreme GC regions. Thus genuine variants in these regions may be missed.
This software attempts to use short kmer frequencies to generate an
alernative "normalized" depth (the `NDP` tag) which could be used instead.

## Quick Start

```
% trencha --version
trencha 0.1.2

```

## Installation

### Conda
Install [Bioconda](https://bioconda.github.io/user/install.html) then:
```
conda install -c conda-forge -c bioconda -c defaults trencha # COMING SOON
```

### Homebrew
Install [Homebrew](http://brew.sh/) (MacOS)
or [Linuxbrew](http://linuxbrew.sh/) (Linux) then:
```
brew install brewsci/bio/trencha # COMING SOON
```

### Source
This will install the latest version direct from Github.
You'll need to add the trencha `bin` directory to your `$PATH`,
and also ensure all the [dependencies](#Dependencies) are installed.
```
cd $HOME
git clone https://github.com/tseemann/trencha.git
$HOME/trencha/bin/trencha --help
```

## Dependencies

* `perl` >= 5.26

## License

trencha is free software, released under the
[GPL 3.0](https://raw.githubusercontent.com/tseemann/trencha/master/LICENSE).

## Issues

Please submit suggestions and bug reports to the
[Issue Tracker](https://github.com/tseemann/trencha/issues)

## Author

[Torsten Seemann](https://twitter.com/torstenseemann)
