---
description: DescribeAddressResult schema from Amazon Snow Family API
layout: schema
name: DescribeAddressResult
properties_list:
- description: ''
  name: Address
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-address-result-schema.json
slug: amazon-snow-family-describe-address-result
source_filename: amazon-snow-family-describe-address-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-address-result-schema.json\",\n  \"title\": \"DescribeAddressResult\",\n  \"description\": \"DescribeAddressResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Address\"\n        },\n        {\n          \"description\": \"The address that you want the Snow device(s) associated with a specific job to be shipped to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-address-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeAddressResult
---
