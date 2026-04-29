---
description: The result of a <code>DeleteElasticsearchDomain</code> request. Contains the status of the pending deletion, or no status if the domain and all of its resources have been deleted.
layout: schema
name: DeleteElasticsearchDomainResponse
properties_list:
- description: ''
  name: DomainStatus
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-delete-elasticsearch-domain-response-schema.json
slug: openapi-delete-elasticsearch-domain-response
source_filename: openapi-delete-elasticsearch-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-elasticsearch-domain-response-schema.json\",\n  \"title\": \"DeleteElasticsearchDomainResponse\",\n  \"description\": \"The result of a <code>DeleteElasticsearchDomain</code> request. Contains the status of the pending deletion, or no status if the domain and all of its resources have been deleted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchDomainStatus\"\n        },\n        {\n          \"description\": \"The status of the Elasticsearch domain being deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-elasticsearch-domain-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DeleteElasticsearchDomainResponse
---
