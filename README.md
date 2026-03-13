Ballerina CDC Azure Blob Schema History Driver Library
===================

  [![Build](https://github.com/ballerina-platform/module-ballerinax-cdc.schema.azure.blob.driver/actions/workflows/build-timestamped-master.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinax-cdc.schema.azure.blob.driver/actions/workflows/build-timestamped-master.yml)
  [![Trivy](https://github.com/ballerina-platform/module-ballerinax-cdc.schema.azure.blob.driver/actions/workflows/trivy-scan.yml/badge.svg)](https://github.com/ballerina-platform/module-ballerinax-cdc.schema.azure.blob.driver/actions/workflows/trivy-scan.yml)
  [![GitHub Last Commit](https://img.shields.io/github/last-commit/ballerina-platform/module-ballerinax-cdc.schema.azure.blob.driver.svg)](https://github.com/ballerina-platform/module-ballerinax-cdc.schema.azure.blob.driver/commits/main)
  [![GitHub issues](https://img.shields.io/github/issues/ballerina-platform/ballerina-library/module/cdc.svg?label=Open%20Issues)](https://github.com/ballerina-platform/ballerina-library/labels/module%2Fcdc)

This library provides the necessary drivers required for the CDC (Change Data Capture) connector to use Azure Blob Storage as an internal schema history storage in Ballerina.

## Usage

To include the `cdc.schema.azure.blob.driver` dependency in your project, simply import the module as shown below:

```ballerina
import ballerinax/cdc;
import ballerinax/cdc.schema.azure.blob.driver as _;
```

The library is bundled with the required drivers, so no additional configuration is needed.

## Issues and projects

Issues and Projects tabs are disabled for this repository. To report bugs, request new features, start new discussions, view project boards, etc. please visit Ballerina Library [parent repository](https://github.com/ballerina-platform/ballerina-library).

This repository only contains the source code for the package.

## Build from the source

### Set up the prerequisites

1. Download and install Java SE Development Kit (JDK) version 21 (from one of the following locations).
   * [Oracle](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html)
   * [OpenJDK](https://adoptium.net/)

2. Download and install [Docker](https://www.docker.com/get-started)

### Build the source

Execute the commands below to build from the source.

1. To build the library:

        ./gradlew clean build

2. Publish ZIP artifact to the local `.m2` repository:

        ./gradlew clean build publishToMavenLocal

3. Publish the generated artifacts to the local Ballerina central repository:

        ./gradlew clean build -PpublishToLocalCentral=true

4. Publish the generated artifacts to the Ballerina central repository:

        ./gradlew clean build -PpublishToCentral=true

## Contribute to Ballerina

As an open source project, Ballerina welcomes contributions from the community.

For more information, go to the [contribution guidelines](https://github.com/ballerina-platform/ballerina-lang/blob/master/CONTRIBUTING.md).

## Code of conduct

All contributors are encouraged to read the [Ballerina code of conduct](https://ballerina.io/code-of-conduct).

## Useful links

* For more information go to the [`cdc.schema.azure.blob.driver` library](https://lib.ballerina.io/ballerinax/cdc.schema.azure.blob.driver/latest).
* For example demonstrations of the usage, go to [Ballerina By Examples](https://ballerina.io/learn/by-example/#database-access).
* Chat live with us via our [Discord server](https://discord.gg/ballerinalang).
* Post all technical questions on Stack Overflow with the [#ballerina](https://stackoverflow.com/questions/tagged/ballerina) tag.
