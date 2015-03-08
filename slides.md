# The DrupalCI initiative

![DrupalCI](./assets/logo.png "DrupalCI")

---

# The future of Drupal.org CI

![DrupalCI](./assets/logo.png "DrupalCI")

---

## Overview

* What is CI?
* The origin story of Drupal and CI
* The state of Drupal and CI
* DrupalCI
* Components
* Questions and DEMANDS!!!!

---

## Me

* Nick Schuch (nick_schuch)
* PreviousNext
* Developer / Sys ops
* PHP, Golang, Docker, Puppet (All the techs!)
* Maintainer Tour module (Drupal 8)
* Maintainer of DrupalCI compontents
	* API
	* Dispatcher
	* Results

---

## Stop me if I go to fast

![DrupalCI](./assets/logo.png "DrupalCI")

---

## Continuous integration

Continuous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day. Each check-in is then verified by an automated build, allowing teams to detect problems early.

---

## Current

* Patch workflow
* Drupal site to manage builds (https://qa.drupal.org/pifr/status)
* Puppet manifest for "nodes" built by people
* Only test one version
* No tests for the infrastructure
* Locked into simpletest

---

## Goals

* Unlock better testing
* Leverage industry standards
* Less custom code
* More versions
* Provide tools for better testing
* Automate everything
* Test our own code
* Ship as images for Vagrant / AWS / Docker

---

## The main goal

* Build for the community

---

## Technologies

![DrupalCI](./assets/logo.png "DrupalCI")

---

## Vagrant

![Vagrant](./assets/vagrant.jpg "Vagrant")

---

## Packer

![Packer](./assets/packer.jpg "Packer")

---

## Docker

![Docker](./assets/docker.png "Docker")

---

## Jenkins

![Docker](./assets/jenkins.png "Jenkins")

---

## Components

![Components](./assets/components.jpg "Components")

---

## Diagram

![Diagram](./assets/diagram.png "Diagram")

---

## API

* Silex (Symfony micro framework)
* Abstraction layer
* Drupal.org / CLI integration point
* Multiple providers
* Does one thing well
* Urls
	* https://www.drupal.org/project/drupalci_api
	* https://github.com/drupalci/api

---

## Demo

![DrupalCI](./assets/logo.png "DrupalCI")

---

## Dispatcher

* Jenkins
* Queues builds
* Starts the "Job runner" component
* More than one provider
* Packaging status
 * Vagrant
 * AWS AMI
* Urls
	* https://www.drupal.org/project/drupalci_dispatcher
	* https://github.com/drupalci/dispatcher

---

## Job Runner

* The DrupalCI workflow
* Symfony console
* Spins up containers (Docker)
* Runs the test script
* Packaged as a PHAR
* Postgres / mongo
* Urls
	* https://www.drupal.org/project/drupalci_testbot
	* https://github.com/drupalci/runner (empty)

---

## Demo

![DrupalCI](./assets/logo.png "DrupalCI")

---

## PrivateTravis

* Compatibilty layer
* Symfony console
* Brings back projects running on Github
* Enables existing projects to have all the benefits of Travis
* Urls
	* https://github.com/nickschuch/PrivateTravis

---

## Results

* Extremely important
* Built on Drupal 8
* CLI built on Symfony console
* All records / artefacts driven by CLI
* CLI generates the famous **1 Passed, 1000000 failed** message
* Urls
	* https://www.drupal.org/project/drupalci_results
	* https://github.com/drupalci/results

---

## Results - Latest

![Latest](./assets/latest.png "Latest")

---

## Results - Build

![Build](./assets/build.png "Build")

---

## Demo

![DrupalCI](./assets/logo.png "DrupalCI")

---

## Project ideas

* A gist.github.com like service
* Drush command

---

## Call to arms

* DrupalSouth sprints - This Saturday
* D8 Accelerate sprints - March 31st to April 2nd (Ill be sprinting that entire week)

---

## Contact

* **Weekly Hangout**: 
 * Google hangout - http://bit.ly/1sBysAN
 * Timezone - https://bitly.com/shorten/

* **IRC**: #drupal-testing.
 * Jeremy Thorson - jthorson
 * Nick Schuch - nick_schuch
 * Ricardo Amaro - ricardoamaro

---

## Questions and DEMANDS!!!

![DrupalCI](./assets/logo.png "DrupalCI")

---

## Resources

* https://www.previousnext.com.au/blog/drupalci-results-component
* https://www.previousnext.com.au/blog/if-you-it-then-you-should-put-phing-it
* Runner component screencast coming soon!
