---
description: ProjectsList schema from AWS CodeStar API
layout: schema
name: ProjectsList
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-projects-list-schema.json
slug: codestar-projects-list
source_filename: codestar-projects-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-projects-list-schema.json\",\n  \"title\": \"ProjectsList\",\n  \"description\": \"ProjectsList schema from AWS CodeStar API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ProjectSummary\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-projects-list-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ProjectsList
---
