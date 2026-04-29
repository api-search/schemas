---
description: DescribeAddressRequest schema from Amazon Snow Family API
layout: schema
name: DescribeAddressRequest
properties_list:
- description: ''
  name: AddressId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-address-request-schema.json
slug: amazon-snow-family-describe-address-request
source_filename: amazon-snow-family-describe-address-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-address-request-schema.json\",\n  \"title\": \"DescribeAddressRequest\",\n  \"description\": \"DescribeAddressRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a specific address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AddressId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-address-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeAddressRequest
---
