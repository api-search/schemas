---
description: DescribeAddressesResult schema from Amazon Snow Family API
layout: schema
name: DescribeAddressesResult
properties_list:
- description: ''
  name: Addresses
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-addresses-result-schema.json
slug: amazon-snow-family-describe-addresses-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-addresses-result-schema.json\",\n  \"title\": \"DescribeAddressesResult\",\n  \"description\": \"DescribeAddressesResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressList\"\n        },\n        {\n          \"description\": \"The Snow device shipping addresses that were created for this account.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. If you use the automatically generated <code>NextToken</code> value in your next <code>DescribeAddresses</code> call, your list\
  \ of returned addresses will start from this point in the array.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-addresses-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeAddressesResult
---
