---
description: Specifies the zone awareness configuration for the domain cluster, such as the number of availability zones.
layout: schema
name: ZoneAwarenessConfig
properties_list:
- description: ''
  name: AvailabilityZoneCount
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-zone-awareness-config-schema.json
slug: openapi-zone-awareness-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-zone-awareness-config-schema.json\",\n  \"title\": \"ZoneAwarenessConfig\",\n  \"description\": \"Specifies the zone awareness configuration for the domain cluster, such as the number of availability zones.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZoneCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"An integer value to indicate the number of availability zones for a domain when zone awareness is enabled. This should be equal to number of subnets if VPC endpoints is enabled\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-zone-awareness-config-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ZoneAwarenessConfig
---
