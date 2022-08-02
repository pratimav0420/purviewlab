# Module 15 - PyApacheAtlas using Azure Databricks

[< Previous Module](../modules/module09.md) - **[Home](../README.md)** - [Next Module >](../modules/module11.md)

## :loudspeaker: Introduction

In the previous module we have seen using Rest API inorder to create Purview assets. In this module we will introduce you to using the Pyapache atlas SDK to programmatically interact with Purview. Spark and Python are now becoming the defacto standard for data processing and the Pyapache atlas SDK provides easy to use packages for programmatic creation of spark assets and interaction with the purview workspace. The SDK provides relevant methods to:

* Authenticate to Microsoft Purview using Service Principal
* Creating Entities, Relationships and performing updates 
* Working with classifications.
* Extracting Purview assests for dependency management.

The primary focus of this module is to be able to create Spark Entity types or that are not available out of the box in the purview workspace or create  other assets that may be specific to an organization that require customization.

## :thinking: Prerequisites

* An [Azure account](https://azure.microsoft.com/free/) with an active subscription.
* A Microsoft Purview account (see [module 01](../modules/module01.md)).
* Completion of steps 2, 3 and 4 from Module 10 (see [module 10](../modules/module10.md))

## :hammer: Tools

* [PyApacheAtlas](https://pypi.org/project/pyapacheatlas/) (will be used to download the library into Azure databricks)

## :dart: Objectives

* Understand the high-level PyApache Atlas SDK.
* Authenticate into Microsoft Purview from Azure Databricks.
* Create (custom) spark entities.
* Associate the entities and establish relationships during data processing

## Table of Contents
1. [PyApache Atlas SDK](#1-Pyapache-atlas-SDK)
2. [Register an Application, Generate a client secret and provide access](#2-register-an-application)
3. Provide service principal access to Storage account
3. Create and launch Databricks workspace
4. Create a spark cluster
6. Download the Pyapache Library to the cluster
7. Create a Notebook
8. Import the relevant packages and Connect to the Purview workspace from the databricks spark environment
9. Create a dataframe from an existing databricks dataset
10. Create a custom entity type to represent a spark dataframe



