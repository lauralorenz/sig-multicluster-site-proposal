# Multicluster Services API Overview

This document provides an overview of Multicluster Services API.

This is an extension of the Services concept across multiple clusters. Services are the basic way that workloads communicate with each other in Kubernetes, and the Multicluster Services builds upon the [Namespace Sameness](namespace-sameness.md) concept to extend Services across multiclusters. In short, Services can remain available across clusters simply by using the same names. The Control Plane can be centralized or decentralized, but consumers only even rely on local data.

This document solely focuses on the API and the common behaviour, leaving room for various [implementations](../implementations.md). There is no reference implementation available.

ClusterIP and headless services just work as expected across clusters.



## Roles and personas.


## Resource model


## Examples