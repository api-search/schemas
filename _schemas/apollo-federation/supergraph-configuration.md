---
description: JSON Schema for Apollo Router and Federation supergraph configuration (supergraph.yaml / router.yaml).
layout: schema
name: Apollo Federation Supergraph Configuration
properties_list:
- description: Federation version for composition.
  name: federation_version
  type: string
- description: Subgraph definitions keyed by name.
  name: subgraphs
  type: object
provider_name: Apollo Federation
provider_slug: apollo-federation
schema_file: json-schema/supergraph-configuration.json
slug: supergraph-configuration
tags:
- API Gateway
- Federation
- GraphQL
- Microservices
- Open Source
- Subgraphs
- Supergraph
title: Apollo Federation Supergraph Configuration
---
