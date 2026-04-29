---
description: Response containing list of all Geode regions
layout: schema
name: RegionListResponse
properties_list:
- description: List of region descriptors
  name: regions
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-region-list-response-schema.json
slug: geode-rest-region-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-region-list-response-schema.json\",\n  \"title\": \"RegionListResponse\",\n  \"description\": \"Response containing list of all Geode regions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"regions\": {\n      \"type\": \"array\",\n      \"description\": \"List of region descriptors\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RegionInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-region-list-response-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: RegionListResponse
---
