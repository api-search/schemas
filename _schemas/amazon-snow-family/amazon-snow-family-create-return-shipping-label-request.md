---
description: CreateReturnShippingLabelRequest schema from Amazon Snow Family API
layout: schema
name: CreateReturnShippingLabelRequest
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: ShippingOption
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-return-shipping-label-request-schema.json
slug: amazon-snow-family-create-return-shipping-label-request
source_filename: amazon-snow-family-create-return-shipping-label-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-return-shipping-label-request-schema.json\",\n  \"title\": \"CreateReturnShippingLabelRequest\",\n  \"description\": \"CreateReturnShippingLabelRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The ID for a job that you want to create the return shipping label for; for example, <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"The shipping speed for a particular job. This speed doesn't\
  \ dictate how soon the device is returned to Amazon Web Services. This speed represents how quickly it moves to its destination while in transit. Regional shipping speeds are as follows:\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-return-shipping-label-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateReturnShippingLabelRequest
---
