---
description: Physical memory cap statistics
layout: schema
name: MemoryCapStats
properties_list:
- description: Physical memory cap in bytes
  name: physcap
  type: integer
- description: Current resident set size in bytes
  name: rss
  type: integer
- description: Number of times memory went over the cap
  name: nover
  type: integer
- description: Total bytes paged out due to capping
  name: pagedout
  type: integer
- description: Pages paged in
  name: pgpgin
  type: integer
- description: Anonymous pages paged in
  name: anonpgin
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-memory-cap-stats-schema.json
slug: solaris-zone-stats-memory-cap-stats
source_filename: solaris-zone-stats-memory-cap-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemoryCapStats\",\n  \"type\": \"object\",\n  \"description\": \"Physical memory cap statistics\",\n  \"properties\": {\n    \"physcap\": {\n      \"type\": \"integer\",\n      \"description\": \"Physical memory cap in bytes\"\n    },\n    \"rss\": {\n      \"type\": \"integer\",\n      \"description\": \"Current resident set size in bytes\"\n    },\n    \"nover\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times memory went over the cap\"\n    },\n    \"pagedout\": {\n      \"type\": \"integer\",\n      \"description\": \"Total bytes paged out due to capping\"\n    },\n    \"pgpgin\": {\n      \"type\": \"integer\",\n      \"description\": \"Pages paged in\"\n    },\n    \"anonpgin\": {\n      \"type\": \"integer\",\n      \"description\": \"Anonymous pages paged in\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-memory-cap-stats-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: MemoryCapStats
---
