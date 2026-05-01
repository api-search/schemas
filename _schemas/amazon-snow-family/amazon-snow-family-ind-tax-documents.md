---
description: The tax documents required in Amazon Web Services Region in India.
layout: schema
name: INDTaxDocuments
properties_list:
- description: ''
  name: GSTIN
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-ind-tax-documents-schema.json
slug: amazon-snow-family-ind-tax-documents
source_filename: amazon-snow-family-ind-tax-documents-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-ind-tax-documents-schema.json\",\n  \"title\": \"INDTaxDocuments\",\n  \"description\": \"The tax documents required in Amazon Web Services Region in India.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GSTIN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GSTIN\"\n        },\n        {\n          \"description\": \"The Goods and Services Tax (GST) documents required in Amazon Web Services Region in India.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-ind-tax-documents-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: INDTaxDocuments
---
