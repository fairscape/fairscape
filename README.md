# Fairscape monorepo

This repo contains all code for all fairscape framework components and clients.


## Abstract 
Results of computational analyses require transparent disclosure of their supporting resources, while the analyses themselves often can be very large scale and involve multiple processing steps separated in time. Evidence for the correctness of any analysis should include not only a textual description, but also a formal record of the computations which produced the result, including accessible data and software with runtime parameters, environment, and personnel involved.  
This repo describes FAIRSCAPE, a reusable computational framework, enabling simplified access to modern scalable cloud-based components. FAIRSCAPE fully implements the FAIR data principles and extends them to provide fully FAIR Evidence, including machine-interpretable provenance of datasets, software and computations, as metadata for all computed results.  
The FAIRSCAPE microservices framework creates a complete Evidence Graph for every computational result, including persistent identifiers with metadata, resolvable to the software, computations, and datasets used in the computation; and stores a URI to the root of the graph in the result’s metadata. An ontology for Evidence Graphs, EVI (https://w3id.org/EVI), supports inferential reasoning over the evidence.  
FAIRSCAPE can run nested or disjoint workflows and preserves provenance across them. It can run Apache Spark jobs, scripts, workflows, or user-supplied containers. All objects are assigned persistent IDs, including software. All results are annotated with FAIR metadata using the evidence graph model for access, validation, reproducibility, and re-use of archived data and software. 

## Documentation

Install instructions, API documentation, and Demo: [HERE](https://fairscape.github.io/)

To download all repostories for this release run:

```shell
git clone --recursive https://github.com/fairscape/fairscape
```

The latest version of each service is also available in their indivdual repostories. 

## Deepnote Demos

The Demos may also be run without installing FAIRSCAPE locally with Deepnote available [HERE](https://deepnote.com/project/Spark-Demo-vDQIIg6CQmi3jnX_N_GYNw/%2FSpark-Demo%2FKubernetes%20Demo-Client.ipynb)
