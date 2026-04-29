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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-region-info-schema.json\",\n  \"title\": \"RegionInfo\",\n  \"description\": \"Metadata about a Geode region\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Region name\",\n      \"example\": \"orders\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Region type (REPLICATE, PARTITION, etc.)\",\n      \"example\": \"PARTITION\"\n    },\n    \"keyConstraint\": {\n      \"type\": \"string\",\n      \"description\": \"Java class constraint for keys, or null\",\n      \"nullable\": \"True\"\n    },\n    \"valueConstraint\": {\n      \"type\": \"string\",\n      \"description\": \"Java class constraint for values, or null\",\n      \"nullable\": \"True\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-region-info-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: RegionInfo
---
