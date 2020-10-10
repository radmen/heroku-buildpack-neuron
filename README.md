# Heroku buildpack: Neuron Zettelkasten

This is a [Heroku buildpack](https://devcenter.heroku.com/articles/buildpacks) for sites powered by [Neuron](https://github.com/srid/neuron). It uses the latest stable version of Neuron.

## Usage

To trigger detection of this build you need to make sure that `neuron.dhall` is in the root directory.

Create a Heroku application using this buildpack:

```
$ heroku create --buildpack https://github.com/radmen/heroku-buildpack-neuron.git
```

or configure your existent application:

```
$ heroku buildpacks:set BUILDPACK_URL="https://github.com/radmen/heroku-buildpack-neuron.git"
```

Then git push to heroku and open your application!

```
$ git push heroku master
$ heroku open
```
