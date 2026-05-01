---
description: The tax documents required in your Amazon Web Services Region.
layout: schema
name: TaxDocuments
properties_list:
- description: ''
  name: IND
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-tax-documents-schema.json
slug: amazon-snow-family-tax-documents
source_filename: amazon-snow-family-tax-documents-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-tax-documents-schema.json\",\n  \"title\": \"TaxDocuments\",\n  \"description\": \"The tax documents required in your Amazon Web Services Region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IND\": {\n      \"$ref\": \"#/components/schemas/INDTaxDocuments\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-tax-documents-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: TaxDocuments
---
