# Changelog

This file contains all the notable changes done to the Ballerina `cdc.schema.azure.blob.driver` package through the releases.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed
- Upgrade Netty to 4.2.20.Final, which fixes GraalVM native image builds on Java 25 failing in `io.netty.util.internal.CleanerJava24Linker` (its FFM `malloc`/`free` downcalls are not supported in a native image).

## [1.2.2]

### Changed
- Fix the Azure Blob schema history in GraalVM native images by registering the Azure SDK storage error classes for reflection, which the SDK uses when a container does not exist yet.

## [1.2.1]

### Changed
- Update the bundled Azure SDK to `azure-core` 1.61.0 (with `azure-storage-blob` 12.37.2 and `azure-identity` 1.19.0), which no longer forces `org.slf4j.LoggerFactory` to build-time initialization in GraalVM native images

## [1.2.0]

### Changed
- Update Netty to 4.2.18.Final and Reactor Netty to 1.3.7, replacing `netty-codec` with `netty-codec-base` ([#9152](https://github.com/ballerina-platform/ballerina-library/issues/9152))
- Update the minimum required Ballerina distribution to 2201.14.0 (Swan Lake Update 14) with Java 25 support

## [1.1.1]

### Changed
- Update the bundled Azure SDK to `azure-core` 1.60.0 (with `azure-storage-blob` 12.36.1 and `azure-identity` 1.18.7) and Reactor to 3.7.19 / Reactor Netty 1.2.18. `azure-core` 1.59.0+ no longer forces `org.slf4j.LoggerFactory` to build-time initialization in GraalVM native images
- Update Netty to 4.1.138.Final to address CVE-2026-75595, CVE-2026-75596 and CVE-2026-59903

## [1.1.0]

### Changed
- Upgrade the bundled Debezium Azure Blob schema-history storage to 3.5.1.Final.
