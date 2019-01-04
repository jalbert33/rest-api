# REST API

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Build Status](https://travis-ci.org/symlex/stream-sampler.png?branch=master)](https://travis-ci.org/symlex/stream-sampler)
[![Documentation](https://readthedocs.org/projects/symlex-docs/badge/?version=latest&style=flat)](https://docs.symlex.org/en/latest/)

This is an example REST API application based on [Symlex Core](https://github.com/symlex/symlex-core).

*Note: https://github.com/symlex/symlex-core contains the kernel and routers as reusable components.*

## Setup ##

Before you start, make sure you have PHP 7.1+, Composer and Docker installed on your system 
(short [howto](https://docs.symlex.org/en/latest/osx/) for Mac OS X users). 
Instead of using Docker, you can also setup your own runtime environment based on the existing 
[Docker configuration](https://github.com/symlex/symlex/tree/master/app/docker).

**Step 1:** Run [Composer](https://getcomposer.org/) to create a new Symlex project:

```
composer create-project symlex/rest-api myapp
```

**Step 2:** Start nginx and PHP using [Docker](https://www.docker.com/):

```
cd myapp
docker-compose up
```

**Step 3:** Open http://localhost:8088/example/123 in a browser ([source](src/Controller/ExampleController.php)).

Our complete framework documentation can be found on [docs.symlex.org](https://docs.symlex.org/en/latest/).

## About ##

Symlex is maintained by [Michael Mayer](https://blog.liquidbytes.net/about/) and
aims to simplify agile Web development by providing a working system that promotes best practices by example.
Michael released his [first PHP framework](http://freshmeat.sourceforge.net/projects/awf) in 2001 and 
has worked with various major framework vendors in the past.
Building this would not have been possible without a lot of prior work by other developers.
Thank you to those and everyone who contributed!

> Choice is the enemy of productivity. Put another way, if your solution does everything, 
> and has no opinions about anything, then it solves nothing. ― *Asim Aslam*

Feel free to send an e-mail to [hello@symlex.org](mailto:hello@symlex.org) if you have any questions, 
need [commercial support](https://blog.liquidbytes.net/contact/) or just want to say hello. 
We welcome contributions of any kind. If you have a bug or an idea, read our 
[guide](https://docs.symlex.org/en/latest/contribute/) before opening an issue.