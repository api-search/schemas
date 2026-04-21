---
description: Metadata about a Geode region
layout: schema
name: RegionInfo
properties_list:
- description: Region name
  name: name
  type: string
- description: Region type (REPLICATE, PARTITION, etc.)
  name: type
  type: string
- description: Java class constraint for keys, or null
  name: keyConstraint
  type: string
- description: Java class constraint for values, or null
  name: valueConstraint
  type: string
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-region-info-schema.json
slug: geode-rest-region-info
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: RegionInfo
---
