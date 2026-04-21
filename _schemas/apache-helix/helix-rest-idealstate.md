---
description: Desired ideal state for resource partition placement
layout: schema
name: IdealState
properties_list:
- description: Resource name
  name: id
  type: string
- description: State model reference
  name: stateModelDefRef
  type: string
- description: Map of partition to desired instance state map
  name: mapFields
  type: object
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-idealstate-schema.json
slug: helix-rest-idealstate
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: IdealState
---
