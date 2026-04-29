---
description: Information about the configuration of an integrated development environment (IDE) for a Dev Environment.
layout: schema
name: IdeConfiguration
properties_list:
- description: ''
  name: runtime
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-ide-configuration-schema.json
slug: amazon-codecatalyst-ide-configuration
source_filename: amazon-codecatalyst-ide-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-ide-configuration-schema.json\",\n  \"title\": \"IdeConfiguration\",\n  \"description\": \"Information about the configuration of an integrated development environment (IDE) for a Dev Environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runtime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeConfigurationRuntimeString\"\n        },\n        {\n          \"description\": \"<p>A link to the IDE runtime image. </p> <note> <p>This parameter is not required for <code>VSCode</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdeConfigurationNameString\"\n        },\n        {\n          \"description\": \"The name of the IDE. Valid values include\
  \ <code>Cloud9</code>, <code>IntelliJ</code>, <code>PyCharm</code>, <code>GoLand</code>, and <code>VSCode</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-ide-configuration-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: IdeConfiguration
---
