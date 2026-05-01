---
description: <p/>
layout: schema
name: ListDiscoveredResourcesResponse
properties_list:
- description: ''
  name: resourceIdentifiers
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-discovered-resources-response-schema.json
slug: config-list-discovered-resources-response
source_filename: config-list-discovered-resources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-discovered-resources-response-schema.json\",\n  \"title\": \"ListDiscoveredResourcesResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdentifierList\"\n        },\n        {\n          \"description\": \"The details that identify a resource that is discovered by Config, including the resource type, ID, and (if available) the custom resource name.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-discovered-resources-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ListDiscoveredResourcesResponse
---
