---
description: CreateReturnShippingLabelResult schema from Amazon Snow Family API
layout: schema
name: CreateReturnShippingLabelResult
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-return-shipping-label-result-schema.json
slug: amazon-snow-family-create-return-shipping-label-result
source_filename: amazon-snow-family-create-return-shipping-label-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-return-shipping-label-result-schema.json\",\n  \"title\": \"CreateReturnShippingLabelResult\",\n  \"description\": \"CreateReturnShippingLabelResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingLabelStatus\"\n        },\n        {\n          \"description\": \"The status information of the task on a Snow device that is being returned to Amazon Web Services.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-return-shipping-label-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateReturnShippingLabelResult
---
