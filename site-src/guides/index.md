# Implementations

This document tracks downstream implementations and integrations of Multicluster API and provides status and resource references for them.

Implementors and integrators of Multicluster API are encouraged to update this document with status information about their implementations, the versions they cover, and documentation to help users get started.

## Implementation Status


- [Google Cloud MCS][gke-mcs] (General Availability)
- [Submariner] (???)

## Implementations

In this section you will find specific links to blog posts, documentation and other Multicluster API references for specific implementations.


### Google Kubernetes Engine

[Google Kubernetes Engine (GKE)][gke] is a managed Kubernetes platform offered by Google Cloud. GKE's implementation of the Multicluster API is through the [GKE Multi Cluster Service][gke-mcs].

[gke]:https://cloud.google.com/kubernetes-engine
[gke-mcs]:https://cloud.google.com/kubernetes-engine/docs/concepts/multi-cluster-services

Please follow this [guide][gke-mcs-guide] for the first steps to set up multicluster services on GKE.

[gke-mcs-guide]:gke-mcs.md

### Submariner

[Submariner][submariner] is an open-source project enabling direct networking between Pods and Services in different Kubernetes clusters, either on-premises or in the cloud.
Submariner provides:

- Cross-cluster L3 connectivity using encrypted and unencrypted connections
- Service Discovery across clusters
- `subctl`, a command-line utility that simplifies deployment and management
- Support for interconnecting clusters using overlapping CIDRs


[submariner]: https://submariner.io/

