---
description: ''
layout: schema
name: SearchImageSetsRequest
properties_list:
- description: ''
  name: searchCriteria
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-search-image-sets-request-schema.json
slug: healthimaging-search-image-sets-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-image-sets-request-schema.json\",\n  \"title\": \"SearchImageSetsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"searchCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchCriteria\"\n        },\n        {\n          \"description\": \"The search criteria that filters by applying a maximum of 1 item to <code>SearchByAttribute</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-image-sets-request-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: SearchImageSetsRequest
---
