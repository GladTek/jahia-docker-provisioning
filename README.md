<a href="https://www.jahia.com/">
    <img src="https://www.jahia.com/modules/jahiacom-templates/images/jahia-3x.png" alt="Jahia logo" title="Jahia" align="right" height="60" />
</a>

# Provisioning Samples (Not Official just customisation of the initial tutorial repository)

Starting with version 8.0.3.0, Jahia comes with a provisioning API to facilitate the orchestration of Jahia environments. 

Its main objective is to automate the startup of complex environment starting from published Jahia releases. When using the provisioning API, Jahia will be able to reach "production" without requiring manual actions nor direct filesystem access to the Jahia environment.

Primariraly aimed at containerized environments (i.e. Docker) this API is not tied to Docker and is also available on local Jahia installation.

## K8S custom local manifests
Kubernetes custom configuration manifests (to run those examples below) can be found in https://github.com/GladTek/jahia-k8s-provisioning

## In this repository

Each folder in this repository contains all the necessary elements to start a Jahia environment following different use cases. 

These examples serve as proof-of-principles and are not meant at being used "as-is" for production environment.

| Tutorial                                            | Description                                                                                                 |
|-----------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
| [00-start-jahia](./00-start-jahia/)                 | Start Jahia Enterprise with Docker                                                                          |
| [01-personal-api-tokens](./01-personal-api-tokens/) | With a local DerbyBD database, install the `Personal API Tokens` module and create a token                  |
| [02-digitall-mariadb](./02-digitall-mariadb)        | With a MariaDB database, install `Digitall`                                                                 |
| [025-luxe-mariadb](./025-luxe-mariadb)              | With a MariaDB database, install `LuXE` a template set made with new Jahia NPM modules __(GraalVM)__ needed |

__Reminder__: Jahia root credentials are `root / WeLiveInATwilightWorld` for these Docker Compose (passwords and data are here for fun purpose only __change them__).
Jahia default root credentials are `root / root1234` for simple docker run commands 

__03-augmented-search__ and __04-jexperience__ examples are removed intentionally since https://store.jahia.com/nexus/content/repositories/jahia-public-app-store@id=JahiaStore is not accessible for now. Will get back once resolved or changed

## Prerequisites

In order to follow these tutorials you will need the Docker Engine installed on your machine. 

These tutorials expose set ports (such as 9000), you will need to make sure these do not conflict with other resources you might have running on your machine.

__Note__: Please ensure that your Docker installation allows allocating up to 4GB of memory to a container. For MacOS users, in Docker go to Preferences>Advanced and set the memory limit to 4GB or more instead of the default 2GB.

## Get started

Ready to get started? If you're new to Jahia with Docker, you should begin with the [first tutorial](./00-start-jahia/).

## Documentation

The provisioning API is documented on the Academy [here](https://academy.jahia.com/documentation/system-administrator/dev-ops/provisioning/about-provisioning)

More details about the Maven protocol [here](https://ops4j1.jira.com/wiki/spaces/paxurl/pages/3833866/Mvn+Protocol)
