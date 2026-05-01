---
description: Information about the configuration of a Dev Environment session.
layout: schema
name: DevEnvironmentSessionConfiguration
properties_list:
- description: ''
  name: sessionType
  type: object
- description: ''
  name: executeCommandSessionConfiguration
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-dev-environment-session-configuration-schema.json
slug: amazon-codecatalyst-dev-environment-session-configuration
source_filename: amazon-codecatalyst-dev-environment-session-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-session-configuration-schema.json\",\n  \"title\": \"DevEnvironmentSessionConfiguration\",\n  \"description\": \"Information about the configuration of a Dev Environment session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentSessionType\"\n        },\n        {\n          \"description\": \"The type of the session.\"\n        }\n      ]\n    },\n    \"executeCommandSessionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecuteCommandSessionConfiguration\"\n        },\n        {\n          \"description\": \"Information about optional commands that will be run on the Dev Environment when the SSH session begins.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"sessionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-session-configuration-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: DevEnvironmentSessionConfiguration
---
