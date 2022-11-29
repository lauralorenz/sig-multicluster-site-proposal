# Introduction

## What is the Multicluster API?

Multicluster API is an open source project managed by the [SIG-Multicluster][sig-multicluster] community. It is a collection of resources and APIs that aim to ease exposing services across Kubernetes clusters.

![Alt](/images/mcs-overview.png "Multicluster API Overview")

### Why the Multicluster API?

With the increased popularity of Kubernetes, many organizations and users have started deploying many Kubernetes clusters and tried to make services communicate across the cluster boundaries. There are many reasons to want to run multiple clusters, including but not limited to:

- Location:
    - Latency: run the application as close to the end-users as possible.
    - Jurisdiction: requirement to keep the user data in-county.
    - Data gravity: data is difficult to move and cluster needs to be deployed next to it.
- Isolation:
    - Environments: many organizations choose to separate development, test and production environments.
    - Performance isolation: it can be required to isolate performance-sensitive applications from other applications.
    - Security isolation: the namespace "soft" boundary is not considered sufficient.
    - Billing: separate teams want to have different teams. Chargeback mechanisms can be difficult to implement at the cluster level.
- Reliability:
    - Blast Radius: sensitive applications must be protected from issues triggered by other applications.
    - Infrastructure diversity: an underlying zone, region or provider outage does not bring down the whole system.
    - Scale: the application might be too big to fit within a single cluster.
    - Upgrade: upgrade of the infrastructure for only some parts of the application.

It is admitted that any non-trivial user is eventually going to face one or more of these issues.

### Multicluster API concepts

The Multicluster API aims at:

- Keeping the multicluster experience consistent with the single cluster experience.
- Exposing workloads from multiple clusters to each other.
- Sharing cluster metadata and its place relative to others.
- More generally, breaking down the walls between clusters.

To achieve these goals, the Multicluster API is defined an extension of the Services concept across multiple clusters. Services are the basic way that workloads communicate with each other in Kubernetes, and the Multicluster API builds upon the [Namespace Sameness](concepts/namespace-sameness.md) concept to extend Services across multiclusters. In short, Services can remain available across clusters simply by using the same names.
The Multicluster API provides three types of resources:

- [ClusterSet](/api-types/cluster-set.md): A collection of clusters that are working together. Each cluster has a unique idenity within the set of clusters. The ClusterSet has also a unique identifier.
- [ServiceExport](/api-types/service-export.md): An interface to export a given service in a specified namespace.
- [ServiceImport](/api-types/service-import.md): An interface to define a service in an external cluster which has been exported.

!!! note

        Exposing services across clusters will require mechanisms similar to a Service Discovery service as well as a registry to store the different cluster identities. In order to broaden the industry support, no reference implementation is provided and Vendors are therefore free to provide their own implementations.



## Getting started

Whether you are a user interested in using the Multicluster API or an implementer 
interested in conforming to the API, the following resources will help give you the necessary background:

- [User guide & Implementations](/guides)
- [API reference spec](/references/spec.md)
- [Community links](/contributing) and [developer guide](/contributing/devguide)


## Who is working on Multicluster API?

The Multicluster API is a
[SIG-Multicluster](SIG-Multicluster)
project being built to improve and standardize the management of services shared across several Kubernetes clusters. 
Current and in-progress implementations include Google Kubernetes Engine (GKE) and Submariner.
Check out the [implementationsreference](implementations.md) to see the latest projects & products that support Multicluster API. If you are interested in contributing to or building an implementation using the Multicluster API then don’t hesitate to [get involved!](/contributing/community)

[SIG-Multicluster]: https://github.com/kubernetes/community/tree/master/sig-multicluster

