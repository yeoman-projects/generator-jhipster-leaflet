# generator-jhipster-leaflet [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url]

## Deprecation Notice

This module has not been updated to work with latest JHipster Versions. In Particular there is no angular-x support. There is another module being compatible with angular-x and newer jhipster versions: https://github.com/ultratrail/generator-jhipster-leafletmap

I strongly advice to use that one!

> Install a sample of ui-leaflet maps on your JHipster application.

## Installation

As this is a [JHipster](http://jhipster.github.io/) module, we expect you have JHipster and its related tools already installed.

```bash
npm install -g generator-jhipster-leaflet
```

Then run the module on a JHipster generated application:

```bash
yo jhipster-leaflet
```

## Using Docker

Download the Dockerfile:

```bash
mkdir docker
cd docker
wget https://github.com/yeoman-projects/generator-jhipster-leaflet/raw/master/Dockerfile
```

Build the Docker images:

```bash
docker build -t generator-jhipster-leaflet:latest .
```

Make a folder where you want to generate the Service:

```bash
mkdir service
cd service
```

Run the generator from image to generate service:

```bash
docker run -it --rm -v $PWD:/home/jhipster/app generator-jhipster-leaflet
```

Run and attach interactive shell to the generator docker container to work from inside the running container:

```bash
docker run -it --rm -v $PWD:/home/jhipster/app generator-jhipster-leaflet /bin/bash
```

## Usage

![](usage.gif)

![resulting html][result-image]

## Angular Leaflet Maps
Angular Leaflet Maps is a set of directives (part of angular-ui) providing angular support for [leafletjs](http://leafletjs.com/).
The search plugin uses [leafletsearch](https://github.com/stefanocudini/leaflet-search).

* Angular leaflet: https://github.com/angular-ui/ui-leaflet
* Leaflet Search: http://labs.easyblog.it/maps/leaflet-search/

## Credits

Heavily inspired by [@moifort](https://github.com/moifort) [google maps generator](https://github.com/moifort/generator-jhipster-google-maps)

## License

Apache-2.0 © [Frederik Hahne](http://atomfrede.github.io/shiny-adventure/)

[npm-image]: https://badge.fury.io/js/generator-jhipster-leaflet.svg
[npm-url]: https://npmjs.org/package/generator-jhipster-leaflet
[travis-image]: https://travis-ci.org/atomfrede/generator-jhipster-leaflet.svg?branch=master
[travis-url]: https://travis-ci.org/atomfrede/generator-jhipster-leaflet
[daviddm-image]: https://david-dm.org/atomfrede/generator-jhipster-leaflet.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/atomfrede/generator-jhipster-leaflet
[result-image]: https://raw.githubusercontent.com/atomfrede/generator-jhipster-leaflet/master/screen.png
