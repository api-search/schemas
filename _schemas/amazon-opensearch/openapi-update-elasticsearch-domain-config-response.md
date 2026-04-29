---
description: The result of an <code>UpdateElasticsearchDomain</code> request. Contains the status of the Elasticsearch domain being updated.
layout: schema
name: UpdateElasticsearchDomainConfigResponse
properties_list:
- description: ''
  name: DomainConfig
  type: object
- description: ''
  name: DryRunResults
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-update-elasticsearch-domain-config-response-schema.json
slug: openapi-update-elasticsearch-domain-config-response
source_filename: openapi-update-elasticsearch-domain-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-elasticsearch-domain-config-response-schema.json\",\n  \"title\": \"UpdateElasticsearchDomainConfigResponse\",\n  \"description\": \"The result of an <code>UpdateElasticsearchDomain</code> request. Contains the status of the Elasticsearch domain being updated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchDomainConfig\"\n        },\n        {\n          \"description\": \"The status of the updated Elasticsearch domain. \"\n        }\n      ]\n    },\n    \"DryRunResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRunResults\"\n        },\n        {\n          \"description\": \"Contains result of DryRun. \"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"DomainConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-elasticsearch-domain-config-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: UpdateElasticsearchDomainConfigResponse
---
