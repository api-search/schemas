---
description: List of USDA AMS market news offices.
layout: schema
name: Offices List Response
properties_list:
- description: ''
  name: results
  type: array
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-offices-list-response-schema.json
slug: mars-api-offices-list-response
source_filename: mars-api-offices-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-offices-list-response-schema.json\",\n  \"title\": \"Offices List Response\",\n  \"description\": \"List of USDA AMS market news offices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Office\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-offices-list-response-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Offices List Response
---
