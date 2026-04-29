---
description: Container for the parameters to the <code><a>DescribeElasticsearchDomains</a></code> operation. By default, the API returns the status of all Elasticsearch domains.
layout: schema
name: DescribeElasticsearchDomainsRequest
properties_list:
- description: ''
  name: DomainNames
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-elasticsearch-domains-request-schema.json
slug: openapi-describe-elasticsearch-domains-request
source_filename: openapi-describe-elasticsearch-domains-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domains-request-schema.json\",\n  \"title\": \"DescribeElasticsearchDomainsRequest\",\n  \"description\": \"Container for the parameters to the <code><a>DescribeElasticsearchDomains</a></code> operation. By default, the API returns the status of all Elasticsearch domains.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainNameList\"\n        },\n        {\n          \"description\": \"The Elasticsearch domains for which you want information.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-elasticsearch-domains-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeElasticsearchDomainsRequest
---
