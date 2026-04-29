---
description: Represents information about a provisioned resource.
layout: schema
name: ResourceDescription
properties_list:
- description: The primary identifier for the resource.
  name: Identifier
  type: string
- description: A JSON string representing the current resource property values. The properties returned depend on the resource type schema.
  name: Properties
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloud-control-resource-description-schema.json
slug: cloud-control-resource-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceDescription\",\n  \"type\": \"object\",\n  \"description\": \"Represents information about a provisioned resource.\",\n  \"properties\": {\n    \"Identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The primary identifier for the resource.\"\n    },\n    \"Properties\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON string representing the current resource property values. The properties returned depend on the resource type schema.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloud-control-resource-description-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ResourceDescription
---
