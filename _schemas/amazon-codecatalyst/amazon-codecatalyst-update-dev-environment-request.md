---
description: UpdateDevEnvironmentRequest schema from Amazon CodeCatalyst
layout: schema
name: UpdateDevEnvironmentRequest
properties_list:
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
schema_file: json-schema/amazon-codecatalyst-update-dev-environment-request-schema.json
slug: amazon-codecatalyst-update-dev-environment-request
source_filename: amazon-codecatalyst-update-dev-environment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-dev-environment-request-schema.json\",\n  \"title\": \"UpdateDevEnvironmentRequest\",\n  \"description\": \"UpdateDevEnvironmentRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDevEnvironmentRequestAliasString\"\n        },\n        {\n          \"description\": \"The user-specified alias for the Dev Environment. Changing this value will not cause a restart.\"\n        }\n      ]\n    },\n    \"ides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeConfigurationList\"\n        },\n        {\n          \"description\": \"Information about the integrated development environment (IDE) configured for a Dev\
  \ Environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"<p>The Amazon EC2 instace type to use for the Dev Environment. </p> <note> <p>Changing this value will cause a restart of the Dev Environment if it is running.</p> </note>\"\n        }\n      ]\n    },\n    \"inactivityTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InactivityTimeoutMinutes\"\n        },\n        {\n          \"description\": \"<p>The amount of time the Dev Environment will run without any activity detected before stopping, in minutes. Only whole integers are allowed. Dev Environments consume compute minutes when running.</p> <note> <p>Changing this value will cause a restart of the Dev Environment if it is running.</p> </note>\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A user-specified idempotency token. Idempotency ensures that an API request completes only once. With an idempotent request, if the original request completes successfully, the subsequent retries return the result from the original successful request and have no additional effect.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-dev-environment-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: UpdateDevEnvironmentRequest
---
