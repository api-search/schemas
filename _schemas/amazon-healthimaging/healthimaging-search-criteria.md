---
description: The search criteria.
layout: schema
name: SearchCriteria
properties_list:
- description: ''
  name: filters
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-search-criteria-schema.json
slug: healthimaging-search-criteria
source_filename: healthimaging-search-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-criteria-schema.json\",\n  \"title\": \"SearchCriteria\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchCriteriaFiltersList\"\n        },\n        {\n          \"description\": \"The filters for the search criteria.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The search criteria.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-criteria-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: SearchCriteria
---
