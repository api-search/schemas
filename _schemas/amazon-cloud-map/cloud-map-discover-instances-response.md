---
description: Response for discovering instances.
layout: schema
name: DiscoverInstancesResponse
properties_list:
- description: ''
  name: Instances
  type: array
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-discover-instances-response-schema.json
slug: cloud-map-discover-instances-response
source_filename: cloud-map-discover-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-discover-instances-response-schema.json\",\n  \"title\": \"DiscoverInstancesResponse\",\n  \"description\": \"Response for discovering instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Instances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HttpInstanceSummary\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-discover-instances-response-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: DiscoverInstancesResponse
---
