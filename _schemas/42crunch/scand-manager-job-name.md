---
description: Unique name identifier for a scan job, prefixed with 'scand-'
layout: schema
name: JobName
properties_list: []
provider_name: 42Crunch
provider_slug: 42crunch
schema_file: json-schema/scand-manager-job-name-schema.json
slug: scand-manager-job-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-job-name-schema.json\",\n  \"title\": \"JobName\",\n  \"description\": \"Unique name identifier for a scan job, prefixed with 'scand-'\",\n  \"type\": \"string\",\n  \"pattern\": \"^scand-[0-9a-zA-Z-]{1,36}$\",\n  \"maxLength\": 42,\n  \"minLength\": 7,\n  \"example\": \"scand-48340c78-a76c-475f-aa4a-36fc834b3c02\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-job-name-schema.json
tags:
- API Security
- Platform
- Scanning
- Security
- OpenAPI
- DevSecOps
title: JobName
---
