---
description: StackId schema from AWS CodeStar API
layout: schema
name: StackId
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-stack-id-schema.json
slug: codestar-stack-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-stack-id-schema.json\",\n  \"title\": \"StackId\",\n  \"description\": \"StackId schema from AWS CodeStar API\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:\\\\s]*:cloudformation:[^:\\\\s]+:[0-9]{12}:stack\\\\/[^:\\\\s]+\\\\/[^:\\\\s]+$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-stack-id-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: StackId
---
