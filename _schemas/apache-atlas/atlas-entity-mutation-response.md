---
description: Response from entity create, update, or delete operations.
layout: schema
name: EntityMutationResponse
properties_list:
- description: Map of client-side temporary GUIDs to server-assigned GUIDs.
  name: guidAssignments
  type: object
- description: Map of mutation type (CREATE, UPDATE, DELETE) to list of mutated entity headers.
  name: mutatedEntities
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-entity-mutation-response-schema.json
slug: atlas-entity-mutation-response
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: EntityMutationResponse
---
