---
description: The result of a <code>DescribeElasticsearchDomain</code> request. Contains the status of the domain specified in the request.
layout: schema
name: DescribeElasticsearchDomainResponse
properties_list:
- description: ''
  name: DomainStatus
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-elasticsearch-domain-response-schema.json
slug: openapi-describe-elasticsearch-domain-response
source_filename: openapi-describe-elasticsearch-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domain-response-schema.json\",\n  \"title\": \"DescribeElasticsearchDomainResponse\",\n  \"description\": \"The result of a <code>DescribeElasticsearchDomain</code> request. Contains the status of the domain specified in the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchDomainStatus\"\n        },\n        {\n          \"description\": \"The current status of the Elasticsearch domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domain-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeElasticsearchDomainResponse
---
