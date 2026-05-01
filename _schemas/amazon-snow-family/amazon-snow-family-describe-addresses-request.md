---
description: DescribeAddressesRequest schema from Amazon Snow Family API
layout: schema
name: DescribeAddressesRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-addresses-request-schema.json
slug: amazon-snow-family-describe-addresses-request
source_filename: amazon-snow-family-describe-addresses-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-addresses-request-schema.json\",\n  \"title\": \"DescribeAddressesRequest\",\n  \"description\": \"DescribeAddressesRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListLimit\"\n        },\n        {\n          \"description\": \"The number of <code>ADDRESS</code> objects to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. To identify what object comes \\\"next\\\" in the list of <code>ADDRESS</code> objects, you have the option of specifying a value for <code>NextToken</code>\
  \ as the starting point for your list of returned addresses.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-addresses-request-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeAddressesRequest
---
