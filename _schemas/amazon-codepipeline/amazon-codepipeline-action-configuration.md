---
description: Represents information about an action configuration.
layout: schema
name: ActionConfiguration
properties_list:
- description: ''
  name: configuration
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-configuration-schema.json
slug: amazon-codepipeline-action-configuration
source_filename: amazon-codepipeline-action-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-configuration-schema.json\",\n  \"title\": \"ActionConfiguration\",\n  \"description\": \"Represents information about an action configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationMap\"\n        },\n        {\n          \"description\": \"The configuration data for the action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-configuration-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionConfiguration
---
