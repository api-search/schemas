---
description: Metadata about an Amazon Lookout for Vision project.
layout: schema
name: ProjectMetadata
properties_list:
- description: ''
  name: ProjectArn
  type: object
- description: ''
  name: ProjectName
  type: object
- description: ''
  name: CreationTimestamp
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-project-metadata-schema.json
slug: amazon-lookout-for-vision-project-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-project-metadata-schema.json\",\n  \"title\": \"ProjectMetadata\",\n  \"description\": \"Metadata about an Amazon Lookout for Vision project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the project.\"\n        }\n      ]\n    },\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project.\"\n        }\n      ]\n    },\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n      \
  \  },\n        {\n          \"description\": \"The unix timestamp for the date and time that the project was created. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-project-metadata-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ProjectMetadata
---
