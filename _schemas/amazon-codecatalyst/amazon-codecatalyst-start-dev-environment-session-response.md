---
description: StartDevEnvironmentSessionResponse schema from Amazon CodeCatalyst
layout: schema
name: StartDevEnvironmentSessionResponse
properties_list:
- description: ''
  name: accessDetails
  type: object
- description: ''
  name: sessionId
  type: object
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-start-dev-environment-session-response-schema.json
slug: amazon-codecatalyst-start-dev-environment-session-response
source_filename: amazon-codecatalyst-start-dev-environment-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-start-dev-environment-session-response-schema.json\",\n  \"title\": \"StartDevEnvironmentSessionResponse\",\n  \"description\": \"StartDevEnvironmentSessionResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessDetails\": {\n      \"$ref\": \"#/components/schemas/DevEnvironmentAccessDetails\"\n    },\n    \"sessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartDevEnvironmentSessionResponseSessionIdString\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment session.\"\n        }\n      ]\n    },\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n         \
  \ \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessDetails\",\n    \"spaceName\",\n    \"projectName\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-start-dev-environment-session-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: StartDevEnvironmentSessionResponse
---
