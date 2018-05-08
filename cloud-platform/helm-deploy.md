---
category: cloud-platform
expires: 2018-01-31
---

# Deploying with Helm

## Overview

Helm is a Kubernetes Package Manager that can simplify the process of deploying and managing applications in the Cloud Platform.

This guide will run through the process of creating a Helm chart for an application and then deploying it into the Cloud Platform.

## Prerequisites

This guide assumes the following:

* Kubectl is installed and configured.
* Authentication with the cluster has been established.
* An environment has been created within the Cloud Platform.
* You have the deployment files for your application.

## Installing Helm

Open a new Terminal window and run the following [Brew](https://brew.sh/) command:

`brew install kubernetes-helm`

Initiate Helm. This will make the necessary local configurations and install Tiller on your cluster, in the default namespace:

`helm init`

You will now be able to use Helm to deploy an application to the Cloud Platform.

## Building the Helm chart

### Generating a template chart

With Helm now configure on your machine, you can start the process of creating a Helm chart template.

In a directory of your choice, issue the following command to generate a Helm chart template:

`helm create yourName` - NOTE: `yourName` will be the name of your chart, this can be changed to your liking.

Within your directory, you will now see a new sub-directory with the name of your chart.

### Helm chart structure

Within your newly generated chart, you will find 4 objects at it's root level, 2 files and 2 directories:

* `Chart.yaml`
* `values.yaml`
* `templates`
* `charts`

### 


## Deploying the Helm chart