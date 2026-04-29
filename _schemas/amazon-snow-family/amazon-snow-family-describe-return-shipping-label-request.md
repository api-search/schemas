---
description: DescribeReturnShippingLabelRequest schema from Amazon Snow Family API
layout: schema
name: DescribeReturnShippingLabelRequest
properties_list:
- description: ''
  name: JobId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-return-shipping-label-request-schema.json
slug: amazon-snow-family-describe-return-shipping-label-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-return-shipping-label-request-schema.json\",\n  \"title\": \"DescribeReturnShippingLabelRequest\",\n  \"description\": \"DescribeReturnShippingLabelRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a job, for example <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-return-shipping-label-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeReturnShippingLabelRequest
---
