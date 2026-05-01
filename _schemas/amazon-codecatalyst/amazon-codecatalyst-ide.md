---
description: Information about an integrated development environment (IDE) used in a Dev Environment.
layout: schema
name: Ide
properties_list:
- description: ''
  name: runtime
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-ide-schema.json
slug: amazon-codecatalyst-ide
source_filename: amazon-codecatalyst-ide-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-ide-schema.json\",\n  \"title\": \"Ide\",\n  \"description\": \"Information about an integrated development environment (IDE) used in a Dev Environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runtime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeRuntimeString\"\n        },\n        {\n          \"description\": \"A link to the IDE runtime image.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeNameString\"\n        },\n        {\n          \"description\": \"The name of the IDE.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-ide-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: Ide
---
