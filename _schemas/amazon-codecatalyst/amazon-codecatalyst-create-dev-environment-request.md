---
description: CreateDevEnvironmentRequest schema from Amazon CodeCatalyst
layout: schema
name: CreateDevEnvironmentRequest
properties_list:
- description: ''
  name: repositories
  type: object
- description: ''
  name: clientToken
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
  name: persistentStorage
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-dev-environment-request-schema.json
slug: amazon-codecatalyst-create-dev-environment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-dev-environment-request-schema.json\",\n  \"title\": \"CreateDevEnvironmentRequest\",\n  \"description\": \"CreateDevEnvironmentRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoriesInput\"\n        },\n        {\n          \"description\": \"The source repository that contains the branch to clone into the Dev Environment. \"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A user-specified idempotency token. Idempotency ensures that an API request completes only once. With an idempotent\
  \ request, if the original request completes successfully, the subsequent retries return the result from the original successful request and have no additional effect.\"\n        }\n      ]\n    },\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateDevEnvironmentRequestAliasString\"\n        },\n        {\n          \"description\": \"The user-defined alias for a Dev Environment.\"\n        }\n      ]\n    },\n    \"ides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeConfigurationList\"\n        },\n        {\n          \"description\": \"<p>Information about the integrated development environment (IDE) configured for a Dev Environment.</p> <note> <p>An IDE is required to create a Dev Environment. For Dev Environment creation, this field contains configuration information and must be provided. </p> </note>\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/InstanceType\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instace type to use for the Dev Environment. \"\n        }\n      ]\n    },\n    \"inactivityTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InactivityTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The amount of time the Dev Environment will run without any activity detected before stopping, in minutes. Only whole integers are allowed. Dev Environments consume compute minutes when running.\"\n        }\n      ]\n    },\n    \"persistentStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PersistentStorageConfiguration\"\n        },\n        {\n          \"description\": \"<p>Information about the amount of storage allocated to the Dev Environment. </p> <note> <p>By default, a Dev Environment is configured to have 16GB of persistent storage when created from the Amazon CodeCatalyst\
  \ console, but there is no default when programmatically creating a Dev Environment. Valid values for persistent storage are based on memory sizes in 16GB increments. Valid values are 16, 32, and 64.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instanceType\",\n    \"persistentStorage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-dev-environment-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateDevEnvironmentRequest
---
