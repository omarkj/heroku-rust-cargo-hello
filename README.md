To deploy this application to Heroku, use this button:

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Or, if you'd prefer to use the command line, try running:

``` sh
git clone https://github.com/emk/heroku-rust-cargo-hello.git
cd heroku-rust-cargo-hello
heroku create --buildpack https://github.com/emk/heroku-buildpack-rust.git
git push heroku master
```

This should make a local copy of this application and deploy it to Heroku.

For further instructions, see
[Deploying Rust applications to Heroku, with example code for Iron][instructions].

[instructions]: http://www.randomhacks.net/2014/09/17/deploying-rust-heroku-iron/

### Does this work with the latest version of Rust?

If this is green, then you should be able to install the latest Rust
compiler, run `cargo update` and build this code successfully:

[![Build Status](https://travis-ci.org/emk/heroku-rust-cargo-hello.svg?branch=master)](https://travis-ci.org/emk/heroku-rust-cargo-hello)

(Note that we only check the build once per day, so it's possible that
things have broken since the latest build.)

If the build is failing, you have two choices:

1. Install Rust and Cargo from the URLs listed in the `RustConfig` file and
   refrain from running `cargo update`.
2. Update the code to work with the latest release of Rust.  Please feel
   free to send me a pull request!
