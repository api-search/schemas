---
description: DescribeMitigationActionResponse schema
layout: schema
name: DescribeMitigationActionResponse
properties_list:
- description: ''
  name: actionName
  type: object
- description: ''
  name: actionType
  type: object
- description: ''
  name: actionArn
  type: object
- description: ''
  name: actionId
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: actionParams
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-mitigation-action-response-schema.json
slug: iot-device-defender-describe-mitigation-action-response
source_filename: iot-device-defender-describe-mitigation-action-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-mitigation-action-response-schema.json\",\n  \"title\": \"DescribeMitigationActionResponse\",\n  \"description\": \"DescribeMitigationActionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionName\"\n        },\n        {\n          \"description\": \"The friendly name that uniquely identifies the mitigation action.\"\n        }\n      ]\n    },\n    \"actionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionType\"\n        },\n        {\n          \"description\": \"The type of mitigation action.\"\n        }\n      ]\n    },\n    \"actionArn\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/MitigationActionArn\"\n        },\n        {\n          \"description\": \"The ARN that identifies this migration action.\"\n        }\n      ]\n    },\n    \"actionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionId\"\n        },\n        {\n          \"description\": \"A unique identifier for this action.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role used to apply this action.\"\n        }\n      ]\n    },\n    \"actionParams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionParams\"\n        },\n        {\n          \"description\": \"Parameters that control how the mitigation action is applied, specific to the type of mitigation action.\"\n        }\n      ]\n    },\n    \"creationDate\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the mitigation action was added to your Amazon Web Services accounts.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the mitigation action was last changed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-mitigation-action-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeMitigationActionResponse
---
