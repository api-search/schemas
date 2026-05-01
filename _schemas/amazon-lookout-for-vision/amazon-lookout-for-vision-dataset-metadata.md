---
description: Summary information for an Amazon Lookout for Vision dataset. For more information, see <a>DescribeDataset</a> and <a>ProjectDescription</a>.
layout: schema
name: DatasetMetadata
properties_list:
- description: ''
  name: DatasetType
  type: object
- description: ''
  name: CreationTimestamp
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-dataset-metadata-schema.json
slug: amazon-lookout-for-vision-dataset-metadata
source_filename: amazon-lookout-for-vision-dataset-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-metadata-schema.json\",\n  \"title\": \"DatasetMetadata\",\n  \"description\": \"Summary information for an Amazon Lookout for Vision dataset. For more information, see <a>DescribeDataset</a> and <a>ProjectDescription</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetType\"\n        },\n        {\n          \"description\": \"The type of the dataset.\"\n        }\n      ]\n    },\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The Unix timestamp for the date and time that the dataset was created. \"\n        }\n      ]\n    },\n   \
  \ \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetStatus\"\n        },\n        {\n          \"description\": \"The status for the dataset.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetStatusMessage\"\n        },\n        {\n          \"description\": \"The status message for the dataset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-metadata-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DatasetMetadata
---
