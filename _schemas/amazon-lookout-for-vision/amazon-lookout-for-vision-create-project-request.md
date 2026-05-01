---
description: CreateProjectRequest schema from Amazon Lookout for Vision API
layout: schema
name: CreateProjectRequest
properties_list:
- description: ''
  name: ProjectName
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-create-project-request-schema.json
slug: amazon-lookout-for-vision-create-project-request
source_filename: amazon-lookout-for-vision-create-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-project-request-schema.json\",\n  \"title\": \"CreateProjectRequest\",\n  \"description\": \"CreateProjectRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name for the project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProjectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-project-request-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: CreateProjectRequest
---
