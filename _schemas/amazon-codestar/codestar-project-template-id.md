---
description: ProjectTemplateId schema from AWS CodeStar API
layout: schema
name: ProjectTemplateId
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-project-template-id-schema.json
slug: codestar-project-template-id
source_filename: codestar-project-template-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-template-id-schema.json\",\n  \"title\": \"ProjectTemplateId\",\n  \"description\": \"ProjectTemplateId schema from AWS CodeStar API\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:\\\\s]{0,5}:codestar:[^:\\\\s]+::project-template(\\\\/(github|codecommit))?\\\\/[a-z0-9-]+$\",\n  \"minLength\": 1\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-project-template-id-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ProjectTemplateId
---
