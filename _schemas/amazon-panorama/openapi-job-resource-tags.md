---
description: Tags for a job.
layout: schema
name: JobResourceTags
properties_list:
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-job-resource-tags-schema.json
slug: openapi-job-resource-tags
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-job-resource-tags-schema.json\",\n  \"title\": \"JobResourceTags\",\n  \"description\": \"Tags for a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResourceType\"\n        },\n        {\n          \"description\": \"The job's type.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The job's tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceType\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-job-resource-tags-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: JobResourceTags
---
