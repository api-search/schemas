---
description: DescribeDomainsResponse schema
layout: schema
name: DescribeDomainsResponse
properties_list:
- description: ''
  name: DomainStatusList
  type: array
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
schema_file: json-schema/cloudsearch-describe-domains-response-schema.json
slug: cloudsearch-describe-domains-response
source_filename: cloudsearch-describe-domains-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-describe-domains-response-schema.json\",\n  \"title\": \"DescribeDomainsResponse\",\n  \"description\": \"DescribeDomainsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainStatusList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DomainStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-describe-domains-response-schema.json
tags:
- CloudSearch
- Search
- Full-Text Search
- Managed
title: DescribeDomainsResponse
---
