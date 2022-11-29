# Versioning

## Overview

### Release Channels (e.g. Experimental, Standard)
## Version Indicators

## What can Change

### Patch version (e.g. v0.4.0 -> v0.4.1)

### Minor version (e.g. v0.4.0 -> v0.5.0)

### Major version (e.g. v0.x to v1.0)

## Graduation Criteria

### Resources

#### Alpha -> Beta
A resource to graduate from alpha to beta must meet the following criteria:

* Implemented by several implementations.
* Conformance test framework is in place, with some coverage of basic
  functionality.
* Validation is well thought out.
* Most of the API surface is being exercised by users.
* Approval from subproject owners + KEP reviewers.

#### Beta -> GA

A resource to graduate from beta to GA must meet the following criteria:

* Almost all of the fields and behavior have conformance test coverage.
* Multiple conformant implementations.
* Widespread implementation and usage.
* At least 6 months of soak time as a beta API.
* Approval from subproject owners + KEP reviewers.

### Fields

#### Experimental -> Standard
As described above, field level stability is layered on top of beta and GA
resources (no fields in alpha resources can be considered standard). The
requirements for a field to graduate from experimental to standard depend on the
API version of the resource it is a part of. For a field to be considered
standard, it needs to meet the same criteria of the resource it is contained in.

If a resource has graduated to beta, an experimental field must meet all of the
beta graduation criteria before graduating to standard. Similarly, if a resource
has graduated to GA, a field must meet all of the beta and GA graduation
criteria. There is one slight variation here, instead of 6 months of soak time
as a beta API, a field graduating to standard requires 6 months of soak time as an
experimental field.

## Out of Scope
### Unreleased APIs
This project will have frequent updates to the main branch. There are no
compatibility guarantees associated with code in any branch, including main,
until it has been released. For example, changes may be reverted before a
release is published. For the best results, use the latest published release of
this project.

### Source Code
We do not provide stability guarantees for source code imports. The Interfaces
and behavior may change in an unexpected and backwards-incompatible way in any
future release.

## Supported Versions

This project aims to provide support for a wide range of Kubernetes versions with
consistent upgrade experiences across versions. To accomplish that, we commit to:

1. Support a minimum of the most recent 5 Kubernetes minor versions.
2. Ensure that all standard channel changes between v1beta1 and v1 are fully
   compatible and convertible.
3. Take every possible effort to avoid introduction of a conversion webhook. If
   a conversion webhook needs to be introduced, it will be supported for the
   lifetime of the API, or at least until an alternative is available.
