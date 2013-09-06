# nwatch

Minimalistic utility to run a command when filesystem updates happen. Requires 
Node.js v0.10+.

    $ npm install -g nwatch

## About

Consider this a cross-platform Node.js-powered port of [visionmedia/watch],
and a cross-platform version of the Linux [watch(1)] utility.

## Usage

Invoke `nwatch <command>` to run the given command when any files change in the 
current directory.

This command will re-run `make` every time any file changes:

    $ nwatch make

## --help

    Usage: nwatch [options] <cmd>

    Options:

      -h, --help          output usage information
      -V, --version       output the version number
      -q, --quiet         only output stderr
      -x, --halt          halt on failure
      -d, --dir [dir]     directory to watch
      -b, --before        run the command before watching as well
      -i, --interval <n>  polling interval (in milliseconds) [1000]
      -v, --verbose       show when a command will be ran

## Alternatives

  * [visionmedia/watch] - works exactly the same, except it's a C program.
  * [watch-js] - has more features geared towards web development like 
  LiveReload.

## Acknowledgements

© 2013, Rico Sta. Cruz. Released under the [MIT License].

[MIT License]: http://www.opensource.org/licenses/mit-license.php
[visionmedia/watch]: https://github.com/visionmedia/watch
[watch(1)]: http://linux.die.net/man/1/watch
[watch-js]: https://github.com/stagas/watch-js
