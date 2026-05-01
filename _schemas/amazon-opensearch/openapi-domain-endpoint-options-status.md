---
description: The configured endpoint options for the domain and their current status.
layout: schema
name: DomainEndpointOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-domain-endpoint-options-status-schema.json
slug: openapi-domain-endpoint-options-status
source_filename: openapi-domain-endpoint-options-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-endpoint-options-status-schema.json\",\n  \"title\": \"DomainEndpointOptionsStatus\",\n  \"description\": \"The configured endpoint options for the domain and their current status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainEndpointOptions\"\n        },\n        {\n          \"description\": \"Options to configure endpoint for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \"The status of the endpoint options for the Elasticsearch domain. See <code>OptionStatus</code> for the status information that's included. \"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Options\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-endpoint-options-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DomainEndpointOptionsStatus
---
