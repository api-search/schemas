---
description: The result of a <code>CreateElasticsearchDomain</code> operation. Contains the status of the newly created Elasticsearch domain.
layout: schema
name: CreateElasticsearchDomainResponse
properties_list:
- description: ''
  name: DomainStatus
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-elasticsearch-domain-response-schema.json
slug: openapi-create-elasticsearch-domain-response
source_filename: openapi-create-elasticsearch-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-elasticsearch-domain-response-schema.json\",\n  \"title\": \"CreateElasticsearchDomainResponse\",\n  \"description\": \"The result of a <code>CreateElasticsearchDomain</code> operation. Contains the status of the newly created Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchDomainStatus\"\n        },\n        {\n          \"description\": \"The status of the newly created Elasticsearch domain. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-elasticsearch-domain-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CreateElasticsearchDomainResponse
---
