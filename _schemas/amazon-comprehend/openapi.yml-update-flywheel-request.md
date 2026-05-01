---
description: UpdateFlywheelRequest schema
layout: schema
name: UpdateFlywheelRequest
properties_list:
- description: ''
  name: FlywheelArn
  type: object
- description: ''
  name: ActiveModelArn
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: DataSecurityConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-update-flywheel-request-schema.json
slug: openapi.yml-update-flywheel-request
source_filename: openapi.yml-update-flywheel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-update-flywheel-request-schema.json\",\n  \"title\": \"UpdateFlywheelRequest\",\n  \"description\": \"UpdateFlywheelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel to update.\"\n        }\n      ]\n    },\n    \"ActiveModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the active model version.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend permission to access the flywheel data.\"\n        }\n      ]\n    },\n    \"DataSecurityConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDataSecurityConfig\"\n        },\n        {\n          \"description\": \"Flywheel data security configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlywheelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-update-flywheel-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: UpdateFlywheelRequest
---
