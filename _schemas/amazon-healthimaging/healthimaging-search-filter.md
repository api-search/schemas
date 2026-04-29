---
description: The search filter.
layout: schema
name: SearchFilter
properties_list:
- description: ''
  name: values
  type: object
- description: ''
  name: operator
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-search-filter-schema.json
slug: healthimaging-search-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-filter-schema.json\",\n  \"title\": \"SearchFilter\",\n  \"type\": \"object\",\n  \"required\": [\n    \"values\",\n    \"operator\"\n  ],\n  \"properties\": {\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchFilterValuesList\"\n        },\n        {\n          \"description\": \"The search filter values.\"\n        }\n      ]\n    },\n    \"operator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Operator\"\n        },\n        {\n          \"description\": \"The search filter operator for <code>imageSetDateTime</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The search filter.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-filter-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: SearchFilter
---
