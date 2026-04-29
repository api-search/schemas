---
description: The result of a <code>DescribeElasticsearchDomainConfig</code> request. Contains the configuration information of the requested domain.
layout: schema
name: DescribeElasticsearchDomainConfigResponse
properties_list:
- description: ''
  name: DomainConfig
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-elasticsearch-domain-config-response-schema.json
slug: openapi-describe-elasticsearch-domain-config-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domain-config-response-schema.json\",\n  \"title\": \"DescribeElasticsearchDomainConfigResponse\",\n  \"description\": \"The result of a <code>DescribeElasticsearchDomainConfig</code> request. Contains the configuration information of the requested domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchDomainConfig\"\n        },\n        {\n          \"description\": \"The configuration information of the domain requested in the <code>DescribeElasticsearchDomainConfig</code> request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domain-config-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeElasticsearchDomainConfigResponse
---
