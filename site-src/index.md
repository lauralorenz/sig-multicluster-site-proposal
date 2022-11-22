## What is the Multicluster API?

Multicluster API is an open source project managed by the [SIG-Multicluster][sig-multicluster]
community. It is a collection of resources that model service networking 
in Kubernetes. These resources - `ServiceExport`,`ServiceImport`, `ClusterSet`, etc - aim to evolve Kubernetes service networking through 
expressive, extensible, and role-oriented interfaces that are implemented by 
many vendors and have broad industry support. 

## Getting started

Whether you are a user interested in using the Multicluster API or an implementer 
interested in conforming to the API, the following resources will help give 
you the necessary background:

- [API overview](/concepts/api-overview)
- [User guides](/guides)
- [Multicluster API implementations](/implementations)
- [API reference spec](/references/spec)
- [Community links](/contributing/community) and [developer guide](/contributing/devguide)


## Multicluster API concepts

## Who is working on Multicluster API?

The Multicluster API is a
[SIG-Multicluster](SIG-Multicluster)
project being built to improve and standardize the management of services shared across several Kubernetes clusters. 
Current and in-progress implementations include Google Kubernetes Engine (GKE) and Submariner.
Check out the [implementationsreference](implementations.md) to see the latest projects &
products that support Multicluster API. If you are interested in contributing to or
building an implementation using the Multicluster API then don’t hesitate to [get
involved!](/contributing/community)

[SIG-Multicluster]: https://github.com/kubernetes/community/tree/master/sig-multicluster

