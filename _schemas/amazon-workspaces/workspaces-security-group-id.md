---
description: SecurityGroupId schema from Amazon WorkSpaces API
layout: schema
name: SecurityGroupId
properties_list: []
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-security-group-id-schema.json
slug: workspaces-security-group-id
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"^(sg-([0-9a-f]{8}|[0-9a-f]{17}))$\",\n  \"minLength\": 11,\n  \"maxLength\": 20,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityGroupId\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-security-group-id-schema.json\",\n  \"description\": \"SecurityGroupId schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-security-group-id-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: SecurityGroupId
---
