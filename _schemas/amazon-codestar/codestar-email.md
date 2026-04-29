---
description: Email schema from AWS CodeStar API
layout: schema
name: Email
properties_list: []
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-email-schema.json
slug: codestar-email
source_filename: codestar-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-email-schema.json\",\n  \"title\": \"Email\",\n  \"description\": \"Email schema from AWS CodeStar API\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"^[\\\\w-.+]+@[\\\\w-.+]+$\",\n  \"minLength\": 3,\n  \"maxLength\": 128\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-email-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: Email
---
