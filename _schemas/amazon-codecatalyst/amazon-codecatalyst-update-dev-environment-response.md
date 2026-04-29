---
description: UpdateDevEnvironmentResponse schema from Amazon CodeCatalyst
layout: schema
name: UpdateDevEnvironmentResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: alias
  type: object
- description: ''
  name: ides
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: inactivityTimeoutMinutes
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-update-dev-environment-response-schema.json
slug: amazon-codecatalyst-update-dev-environment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-dev-environment-response-schema.json\",\n  \"title\": \"UpdateDevEnvironmentResponse\",\n  \"description\": \"UpdateDevEnvironmentResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment. \"\n        }\n      ]\n    },\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\
  \n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDevEnvironmentResponseAliasString\"\n        },\n        {\n          \"description\": \"The user-specified alias for the Dev Environment.\"\n        }\n      ]\n    },\n    \"ides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeConfigurationList\"\n        },\n        {\n          \"description\": \"Information about the integrated development environment (IDE) configured for the Dev Environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instace type to use for the Dev Environment. \"\n        }\n      ]\n    },\n    \"inactivityTimeoutMinutes\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/InactivityTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The amount of time the Dev Environment will run without any activity detected before stopping, in minutes. \"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A user-specified idempotency token. Idempotency ensures that an API request completes only once. With an idempotent request, if the original request completes successfully, the subsequent retries return the result from the original successful request and have no additional effect.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"spaceName\",\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-dev-environment-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: UpdateDevEnvironmentResponse
---
