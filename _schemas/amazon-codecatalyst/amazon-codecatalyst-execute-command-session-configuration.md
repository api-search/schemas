---
description: Information about the commands that will be run on a Dev Environment when an SSH session begins.
layout: schema
name: ExecuteCommandSessionConfiguration
properties_list:
- description: ''
  name: command
  type: object
- description: ''
  name: arguments
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-execute-command-session-configuration-schema.json
slug: amazon-codecatalyst-execute-command-session-configuration
source_filename: amazon-codecatalyst-execute-command-session-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-execute-command-session-configuration-schema.json\",\n  \"title\": \"ExecuteCommandSessionConfiguration\",\n  \"description\": \"Information about the commands that will be run on a Dev Environment when an SSH session begins.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecuteCommandSessionConfigurationCommandString\"\n        },\n        {\n          \"description\": \"The command used at the beginning of the SSH session to a Dev Environment.\"\n        }\n      ]\n    },\n    \"arguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecuteCommandSessionConfigurationArguments\"\n        },\n        {\n          \"description\": \"An array of arguments\
  \ containing arguments and members.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"command\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-execute-command-session-configuration-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ExecuteCommandSessionConfiguration
---
