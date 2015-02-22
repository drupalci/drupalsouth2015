# The DrupalCI initiative

![DrupalCI](./assets/logo.png "DrupalCI")

## Overview

* What
* Why
* Current
* Goals
* Components
* Help

## Me

* Nick Schuch
* PreviousNext
* Dev / Sys

## Continuous integration

Continuous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day. Each check-in is then verified by an automated build, allowing teams to detect problems early.

## Current

* Patch workflow
* Drupal site to manage builds (PIFR)
* Puppet manifest for "nodes" done manually
* Only test one version of LAMP
* No tests

## Goals

* Leverage industry standards
* Less custom code
* More versions
* Provide tools for better testing
* Automate everything
* Test our own code
* Ship as images for Vagrant / AWS / Docker

## Goals

Build for the community

## Meet the team

@todo, Get a set of images

## Diagram

![Diagram](./assets/diagram.png "Diagram")

## Components

## Dispatcher

* Jenkins
* Queues builds
* Starts compute if required
* Starts the "Job runner" component
* Packaging status
 * Vagrant - Yes
 * AWS AMI - Yes
 * Docker - No

### Demo

@todo, Record a demo.

## Job Runner

* The DrupalCI workflow
* Symfony console
* Spins up containers (Docker)
* Runs the test script
* Packaged as a PHAR

### Demo

@todo, Record a demo.

### PrivateTravis

* Compatibilty layer
* Symfony console
* Brings back projects running on Github
* Enables existing projects to have all the benefits of Travis

#### Demo

@todo, Record a demo.

## Results

* Extremely important
* Built on Drupal 8
* CLI built on Symfony console
* All records / artefacts driven by CLI
* CLI generates the famous *1 Passed, 1000000 failed* message

### Screenshot - Latest

![Latest](./assets/latest.png "Latest")

### Screenshot - Build

![Build](./assets/build.png "Build")

### Demo

@todo, Record a demo.

## API

* Silex (Symfony micro framework)
* Abstraction layer
* Drupal.org / CLI integration point

### Demo

@todo, Record a demo.

## Drupal.org

Work will begin shortly.

## Metrics

Leverage existing Drupal.org logging.

## Project ideas

* A gist.github.com like service
* Drush command

## Call to arms

@todo, Cool image

## Contact

* **Weekly Hangout**: 
 * Google hangout - http://bit.ly/1sBysAN
 * Timezone - http://www.timeanddate.com/worldclock/fixedtime.html?msg=Modernizing+Testbot+Hangout&iso=20141012T14&p1=210&ah=1

* **IRC**: #drupal-testing.
 * Jeremy Thorson - jthorson
 * Nick Schuch - nick_schuch
 * Ricardo Amaro - ricardoamaro

## Questions