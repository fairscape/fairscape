# FAIRSCAPE Monorepo

**Build AI-Ready Datasets with FAIRSCAPE**

FAIRSCAPE provides a comprehensive framework to ensure your scientific data is not only FAIR but also prepared for AI/ML applications, underpinned by complete provenance through Evidence Graphs for enhanced explainability.

- **AI-Ready**: Primed for ML & Analytics
- **FAIR Foundation**: Findable, Accessible, Interoperable, Reusable
- **Evidence Graphs**: For XAI & Reproducibility

## Framework Overview

FAIRSCAPE is a computational framework written in Python that supports the AI Ready Criteria. It helps prepare components such as datasets, software, computations, runtime parameters, environment, and personnel involved in a computational analysis for AI/ML applications. It generates rich evidence supporting the AI-Readiness and explainability of the analysis by recording formal representations of the components and their interactions in the form of a graph called an Evidence Graph.

For every computational result, FAIRSCAPE creates a machine-interpretable Evidence Graph whose nodes and edges may contain persistent identifiers with metadata resolvable to the underlying components, enhancing transparency and trust in AI-driven insights.

## Components

### FAIRSCAPE Server

The core backend service responsible for metadata management. Implements a RESTful API using FastAPI in Python. This service provides persistent globally unique identifiers (guids) as ARKS for many types of digital objects and maintains provenance metadata crucial for the AI-Readiness and explainability of the data science life-cycle.

### FAIRSCAPE CLI

A data validation and packaging utility for the FAIRSCAPE ecosystem. Provides a command line interface that allows client-side remote teams to create RO-Crates, structuring data for AI applications.

### FAIRSCAPE GUI Client

The FAIRSCAPE Electron App provides a user-friendly interface for packaging research objects and validating metadata, making it easier than ever to ensure your research data is FAIR (Findable, Accessible, Interoperable, and Reusable).

### FAIRSCAPE Web Client

A web-based interface for interacting with the FAIRSCAPE framework, providing accessible tools for managing and validating research data.

## Summary

FAIRSCAPE is a computational framework written in Python that supports the AI Ready Criteria as detailed [here](https://www.biorxiv.org/content/10.1101/2024.10.23.619844v4.full.pdf). It helps prepare components such as datasets, software, computations, runtime parameters, environment, and personnel involved in a computational analysis for AI/ML applications. It generates rich evidence supporting the AI-Readiness and explainability of the analysis by recording formal representations of the components and their interactions in the form of a graph called an Evidence Graph. For every computational result, FAIRSCAPE creates a machine-interpretable Evidence Graph whose nodes and edges may contain persistent identifiers with metadata resolvable to the underlying components, enhancing transparency and trust in AI-driven insights.

FAIRSCAPE provides a command line client tool to package and validate the components with metadata, a schema generation and validation component for the datasets, and a REST API to perform various operations on the server-side.

## Installation

To download all repositories for this release run:

```shell
git clone --recursive https://github.com/fairscape/fairscape
```
