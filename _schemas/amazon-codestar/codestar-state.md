---
description: State schema from AWS CodeStar API
layout: schema
name: State
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-state-schema.json
slug: codestar-state
source_filename: codestar-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-state-schema.json\",\n  \"title\": \"State\",\n  \"description\": \"State schema from AWS CodeStar API\",\n  \"type\": \"string\",\n  \"pattern\": \"^(CreateInProgress|CreateComplete|CreateFailed|DeleteComplete|DeleteFailed|DeleteInProgress|UpdateComplete|UpdateInProgress|UpdateFailed|Unknown)$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-state-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: State
---
