---
description: StopDevEnvironmentSessionResponse schema from Amazon CodeCatalyst
layout: schema
name: StopDevEnvironmentSessionResponse
properties_list:
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: sessionId
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-stop-dev-environment-session-response-schema.json
slug: amazon-codecatalyst-stop-dev-environment-session-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-stop-dev-environment-session-response-schema.json\",\n  \"title\": \"StopDevEnvironmentSessionResponse\",\n  \"description\": \"StopDevEnvironmentSessionResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n\
  \        },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment.\"\n        }\n      ]\n    },\n    \"sessionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopDevEnvironmentSessionResponseSessionIdString\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment session.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spaceName\",\n    \"projectName\",\n    \"id\",\n    \"sessionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-stop-dev-environment-session-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: StopDevEnvironmentSessionResponse
---
