[![Build Status](https://app.travis-ci.com/convenient/travis-debug.svg?branch=main)](https://app.travis-ci.com/convenient/travis-debug)

Travis is failing to install php 7.4 

```
0.01s0.02s$ phpenv global 7.4 2>/dev/null
7.4 is not pre-installed; installing
Downloading archive: https://storage.googleapis.com/travis-ci-language-archives/php/binaries/ubuntu/16.04/x86_64/php-7.4.tar.bz2
11.41s$ curl -sSf --retry 5 -o archive.tar.bz2 $archive_url && tar xjf archive.tar.bz2 --directory /
0.01s0.02s$ phpenv global 7.4
php: error while loading shared libraries: libargon2.so.1: cannot open shared object file: No such file or directory
0.05s$ composer self-update
php: error while loading shared libraries: libargon2.so.1: cannot open shared object file: No such file or directory
$ php --version
php: error while loading shared libraries: libargon2.so.1: cannot open shared object file: No such file or directory
$ composer --version
php: error while loading shared libraries: libargon2.so.1: cannot open shared object file: No such file or directory
0.05s$ php --version
php: error while loading shared libraries: libargon2.so.1: cannot open shared object file: No such file or directory
The command "php --version" exited with 127.
```
