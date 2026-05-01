---
description: keyArn schema from Amazon WorkSpaces Web API
layout: schema
name: keyArn
properties_list: []
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-key-arn-schema.json
slug: workspaces-web-key-arn
source_filename: workspaces-web-key-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"^arn:[\\\\w+=\\\\/,.@-]+:kms:[a-zA-Z0-9\\\\-]*:[a-zA-Z0-9]{1,12}:key\\\\/[a-zA-Z0-9-]+$\",\n  \"minLength\": 20,\n  \"maxLength\": 2048,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"keyArn\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-key-arn-schema.json\",\n  \"description\": \"keyArn schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-key-arn-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: keyArn
---
