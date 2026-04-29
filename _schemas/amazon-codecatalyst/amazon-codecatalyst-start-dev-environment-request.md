---
description: StartDevEnvironmentRequest schema from Amazon CodeCatalyst
layout: schema
name: StartDevEnvironmentRequest
properties_list:
- description: ''
  name: ides
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: inactivityTimeoutMinutes
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-start-dev-environment-request-schema.json
slug: amazon-codecatalyst-start-dev-environment-request
source_filename: amazon-codecatalyst-start-dev-environment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-start-dev-environment-request-schema.json\",\n  \"title\": \"StartDevEnvironmentRequest\",\n  \"description\": \"StartDevEnvironmentRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeConfigurationList\"\n        },\n        {\n          \"description\": \"Information about the integrated development environment (IDE) configured for a Dev Environment. \"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instace type to use for the Dev Environment. \"\n        }\n      ]\n    },\n    \"inactivityTimeoutMinutes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InactivityTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The amount of time the Dev Environment will run without any activity detected before stopping, in minutes. Only whole integers are allowed. Dev Environments consume compute minutes when running.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-start-dev-environment-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: StartDevEnvironmentRequest
---
