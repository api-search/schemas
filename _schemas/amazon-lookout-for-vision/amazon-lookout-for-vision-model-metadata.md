---
description: Describes an Amazon Lookout for Vision model.
layout: schema
name: ModelMetadata
properties_list:
- description: ''
  name: CreationTimestamp
  type: object
- description: ''
  name: ModelVersion
  type: object
- description: ''
  name: ModelArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: Performance
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-model-metadata-schema.json
slug: amazon-lookout-for-vision-model-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-metadata-schema.json\",\n  \"title\": \"ModelMetadata\",\n  \"description\": \"Describes an Amazon Lookout for Vision model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The unix timestamp for the date and time that the model was created. \"\n        }\n      ]\n    },\n    \"ModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelVersion\"\n        },\n        {\n          \"description\": \"The version of the model.\"\n        }\n      ]\n    },\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelArn\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the model.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelDescriptionMessage\"\n        },\n        {\n          \"description\": \"The description for the model.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \"The status of the model.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatusMessage\"\n        },\n        {\n          \"description\": \"The status message for the model.\"\n        }\n      ]\n    },\n    \"Performance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPerformance\"\n        },\n        {\n          \"description\": \"Performance\
  \ metrics for the model. Not available until training has successfully completed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-metadata-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ModelMetadata
---
