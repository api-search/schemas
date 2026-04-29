---
description: ''
layout: schema
name: ListImageSetVersionsResponse
properties_list:
- description: ''
  name: imageSetPropertiesList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-list-image-set-versions-response-schema.json
slug: healthimaging-list-image-set-versions-response
source_filename: healthimaging-list-image-set-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-list-image-set-versions-response-schema.json\",\n  \"title\": \"ListImageSetVersionsResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetPropertiesList\"\n  ],\n  \"properties\": {\n    \"imageSetPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetPropertiesList\"\n        },\n        {\n          \"description\": \"Lists all properties associated with an image set.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the list of image set versions on the next page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-list-image-set-versions-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: ListImageSetVersionsResponse
---
