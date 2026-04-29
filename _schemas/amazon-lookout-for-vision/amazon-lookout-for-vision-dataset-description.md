---
description: The description for a dataset. For more information, see <a>DescribeDataset</a>.
layout: schema
name: DatasetDescription
properties_list:
- description: ''
  name: ProjectName
  type: object
- description: ''
  name: DatasetType
  type: object
- description: ''
  name: CreationTimestamp
  type: object
- description: ''
  name: LastUpdatedTimestamp
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: ImageStats
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-dataset-description-schema.json
slug: amazon-lookout-for-vision-dataset-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-description-schema.json\",\n  \"title\": \"DatasetDescription\",\n  \"description\": \"The description for a dataset. For more information, see <a>DescribeDataset</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project that contains the dataset.\"\n        }\n      ]\n    },\n    \"DatasetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetType\"\n        },\n        {\n          \"description\": \"The type of the dataset. The value <code>train</code> represents a training dataset or single dataset project. The value <code>test</code>\
  \ represents a test dataset.\"\n        }\n      ]\n    },\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The Unix timestamp for the time and date that the dataset was created.\"\n        }\n      ]\n    },\n    \"LastUpdatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The Unix timestamp for the date and time that the dataset was last updated.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetStatus\"\n        },\n        {\n          \"description\": \"The status of the dataset.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetStatusMessage\"\n        },\n        {\n          \"description\"\
  : \"The status message for the dataset. \"\n        }\n      ]\n    },\n    \"ImageStats\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetImageStats\"\n        },\n        {\n          \"description\": \"Statistics about the images in a dataset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-description-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DatasetDescription
---
