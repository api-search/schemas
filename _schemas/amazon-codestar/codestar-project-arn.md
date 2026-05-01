---
description: ProjectArn schema from AWS CodeStar API
layout: schema
name: ProjectArn
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-project-arn-schema.json
slug: codestar-project-arn
source_filename: codestar-project-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-arn-schema.json\",\n  \"title\": \"ProjectArn\",\n  \"description\": \"ProjectArn schema from AWS CodeStar API\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:\\\\s]*:codestar:[^:\\\\s]+:[0-9]{12}:project\\\\/[a-z]([a-z0-9|-])+$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-arn-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ProjectArn
---
