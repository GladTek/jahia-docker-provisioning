# Provisioning Samples (Not Official just customisation of the initial tutorial repository)
Inspired and forked from https://github.com/Jahia/provisioning-tutorials

Those are customisations of the initial Provisioning Tutorials.

What was added :
- more variable configurations in `env` file.
- provisioning in local folder to be sent to docker container for later provisioning instead of an url.
- ability to override a yaml provisioning folder by your own.

## K8S custom local manifests
Kubernetes custom configuration manifests (to run those examples below) can be found in https://github.com/GladTek/jahia-k8s-provisioning

## In this repository

Each folder in this repository contains all the necessary elements to start a Jahia environment following different use cases. 

These examples serve as proof-of-principles and are not meant at being used "as-is" for production environment.

There are two branches

## Branch 8.1

| Sample | Description |
| --- | --- |
| 01-jahia-mariadb-digitall | Jahia 8.1 with Maria DB and Digitall |
| 02-jahia-mariadb-digitall-local-provisioning-files | the previous but with local provisioning files instead of online (with custom module installation)
| 03-jahia-mariadb-digitall-override-folder | Example on how to override patches provisioning folder by a local folder **localMount**

## Branch 8.2

| Sample | Description |
| --- | --- |
| 01-jahia-mariadb-digitall | Jahia 8.2 with Maria DB and Digitall |
| 02-jahia-mariadb-digitall-local-provisioning-files | the previous but with local provisioning files instead of online (with custom module installation)
| 03-jahia-mariadb-digitall-override-folder | Example on how to override patches provisioning folder by a local folder **localMount**)
| 04-jahia-mariadb-luxe | This will create an environment with a website based on an NPM module
| 05-jahia-mariadb-empty | This will create a Jahia 8.2 environment with no website

__Reminder__: Jahia root credentials are `root / WeLiveInATwilightWorld` for these Docker Compose (passwords and data are here for fun purpose only __change them__).

## NB
- __03-augmented-search__ and __04-jexperience__ examples are removed intentionally and temporarily since https://store.jahia.com/nexus/content/repositories/jahia-public-app-store@id=JahiaStore is not accessible for now. Will get back once resolved or changed

- The original sources of this fork for Jahia is in branch **main-backup**

## Prerequisites

In order to follow these tutorials you will need the Docker Engine installed on your machine. 

These tutorials expose set ports (such as 9000), you will need to make sure these do not conflict with other resources you might have running on your machine.

__Note__: Please ensure that your Docker installation allows allocating up to 4GB of memory to a container. For MacOS users, in Docker go to Preferences>Advanced and set the memory limit to 4GB or more instead of the default 2GB.

## Documentation

The provisioning API is documented on the Academy [here](https://academy.jahia.com/documentation/system-administrator/dev-ops/provisioning/about-provisioning)

More details about the Maven protocol [here](https://ops4j1.jira.com/wiki/spaces/paxurl/pages/3833866/Mvn+Protocol)
