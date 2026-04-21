---
description: A relationship between two Atlas entities.
layout: schema
name: AtlasRelationship
properties_list:
- description: GUID of the relationship.
  name: guid
  type: string
- description: Type name of the relationship.
  name: typeName
  type: string
- description: Status of the relationship.
  name: status
  type: string
- description: First endpoint of the relationship.
  name: end1
  type: object
- description: Second endpoint of the relationship.
  name: end2
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-relationship-schema.json
slug: atlas-atlas-relationship
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasRelationship
---
