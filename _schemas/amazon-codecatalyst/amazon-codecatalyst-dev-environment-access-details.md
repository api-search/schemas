---
description: Information about connection details for a Dev Environment.
layout: schema
name: DevEnvironmentAccessDetails
properties_list:
- description: ''
  name: streamUrl
  type: object
- description: ''
  name: tokenValue
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-dev-environment-access-details-schema.json
slug: amazon-codecatalyst-dev-environment-access-details
source_filename: amazon-codecatalyst-dev-environment-access-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-access-details-schema.json\",\n  \"title\": \"DevEnvironmentAccessDetails\",\n  \"description\": \"Information about connection details for a Dev Environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveString\"\n        },\n        {\n          \"description\": \"The URL used to send commands to and from the Dev Environment.\"\n        }\n      ]\n    },\n    \"tokenValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveString\"\n        },\n        {\n          \"description\": \"An encrypted token value that contains session and caller information used to authenticate the connection.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"streamUrl\",\n    \"tokenValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-access-details-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: DevEnvironmentAccessDetails
---
