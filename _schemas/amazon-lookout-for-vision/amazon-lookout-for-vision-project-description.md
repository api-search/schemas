---
description: Describe an Amazon Lookout for Vision project. For more information, see <a>DescribeProject</a>.
layout: schema
name: ProjectDescription
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
- description: ''
  name: Datasets
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-project-description-schema.json
slug: amazon-lookout-for-vision-project-description
source_filename: amazon-lookout-for-vision-project-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-project-description-schema.json\",\n  \"title\": \"ProjectDescription\",\n  \"description\": \"Describe an Amazon Lookout for Vision project. For more information, see <a>DescribeProject</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the project.\"\n        }\n      ]\n    },\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project.\"\n        }\n      ]\n    },\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The unix timestamp for the date and time that the project was created. \"\n        }\n      ]\n    },\n    \"Datasets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetMetadataList\"\n        },\n        {\n          \"description\": \"A list of datasets in the project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-project-description-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ProjectDescription
---
