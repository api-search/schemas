---
description: An indication of whether a project creation or deletion is failed or successful.
layout: schema
name: ProjectStatus
properties_list:
- description: ''
  name: state
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-project-status-schema.json
slug: codestar-project-status
source_filename: codestar-project-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-status-schema.json\",\n  \"title\": \"ProjectStatus\",\n  \"description\": \"An indication of whether a project creation or deletion is failed or successful.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"The phase of completion for a project creation or deletion.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reason\"\n        },\n        {\n          \"description\": \"In the case of a project creation or deletion failure, a reason for the failure.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-status-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ProjectStatus
---
