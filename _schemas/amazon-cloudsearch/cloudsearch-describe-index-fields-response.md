---
description: DescribeIndexFieldsResponse schema
layout: schema
name: DescribeIndexFieldsResponse
properties_list:
- description: ''
  name: IndexFields
  type: array
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
schema_file: json-schema/cloudsearch-describe-index-fields-response-schema.json
slug: cloudsearch-describe-index-fields-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-describe-index-fields-response-schema.json\",\n  \"title\": \"DescribeIndexFieldsResponse\",\n  \"description\": \"DescribeIndexFieldsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IndexFields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Options\": {\n            \"type\": \"object\"\n          },\n          \"Status\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-describe-index-fields-response-schema.json
tags:
- AWS
- CloudSearch
- Search
- Full-Text Search
- Managed
title: DescribeIndexFieldsResponse
---
