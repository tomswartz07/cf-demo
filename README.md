# Pivotal Cloud Foundry Example

## Background
Cloud Foundry is an open source cloud computing platform as a service (PaaS) originally developed by VMware and now overseen by the Cloud Foundry Foundation.
Cloud Foundry was designed and developed by a small team from Google.

Cloud Foundry supports the full lifecycle, from initial development, through all testing stages, to deployment making it well-suited to continuous delivery.
Users have access to one or more spaces, which typically correspond to a lifecycle stage.
For example, an application ready for QA testing might be pushed (deployed) to its project's QA space.

In certain situations, CF can automatically hook into services and set up the required software within the container.
In this example, there is no definition of LAMP, but the PHP file is served on the output address as requested.

## Requirements
- cf-cli
- either PCF account or bosh-lite

## Setup
The code in this repository can be deployed to either a free PCF account, or a local Bosh PCF instance.

```shell
$ cf target <target address> # https://api.bosh-lite.com
$ cf login -u admin -p admin
$ cf push [name] # Name is optional if the manifest.yml file defines it
```


