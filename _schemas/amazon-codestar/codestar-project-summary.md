---
description: Information about the metadata for a project.
layout: schema
name: ProjectSummary
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: projectArn
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-project-summary-schema.json
slug: codestar-project-summary
source_filename: codestar-project-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-summary-schema.json\",\n  \"title\": \"ProjectSummary\",\n  \"description\": \"Information about the metadata for a project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    },\n    \"projectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-summary-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ProjectSummary
---
