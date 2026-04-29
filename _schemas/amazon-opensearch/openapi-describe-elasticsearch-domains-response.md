---
description: The result of a <code>DescribeElasticsearchDomains</code> request. Contains the status of the specified domains or all domains owned by the account.
layout: schema
name: DescribeElasticsearchDomainsResponse
properties_list:
- description: ''
  name: DomainStatusList
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-elasticsearch-domains-response-schema.json
slug: openapi-describe-elasticsearch-domains-response
source_filename: openapi-describe-elasticsearch-domains-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domains-response-schema.json\",\n  \"title\": \"DescribeElasticsearchDomainsResponse\",\n  \"description\": \"The result of a <code>DescribeElasticsearchDomains</code> request. Contains the status of the specified domains or all domains owned by the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainStatusList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchDomainStatusList\"\n        },\n        {\n          \"description\": \"The status of the domains requested in the <code>DescribeElasticsearchDomains</code> request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainStatusList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domains-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeElasticsearchDomainsResponse
---
