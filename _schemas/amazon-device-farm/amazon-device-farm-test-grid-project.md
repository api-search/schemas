---
description: A Selenium testing project. Projects are used to collect and collate sessions.
layout: schema
name: TestGridProject
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: vpcConfig
  type: object
- description: ''
  name: created
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-test-grid-project-schema.json
slug: amazon-device-farm-test-grid-project
source_filename: amazon-device-farm-test-grid-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-project-schema.json\",\n  \"title\": \"TestGridProject\",\n  \"description\": \"A Selenium testing project. Projects are used to collect and collate sessions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceFarmArn\"\n        },\n        {\n          \"description\": \"The ARN for the project.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A human-readable name for the project.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n  \
  \        \"description\": \"A human-readable description for the project.\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestGridVpcConfig\"\n        },\n        {\n          \"description\": \"The VPC security groups and subnets that are attached to a project.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"When the project was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-project-schema.json
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
title: TestGridProject
---
