---
description: ''
layout: schema
name: SearchImageSetsResponse
properties_list:
- description: ''
  name: imageSetsMetadataSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-search-image-sets-response-schema.json
slug: healthimaging-search-image-sets-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-image-sets-response-schema.json\",\n  \"title\": \"SearchImageSetsResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"imageSetsMetadataSummaries\"\n  ],\n  \"properties\": {\n    \"imageSetsMetadataSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSetsMetadataSummaries\"\n        },\n        {\n          \"description\": \"The model containing the image set results.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for pagination results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-search-image-sets-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: SearchImageSetsResponse
---
