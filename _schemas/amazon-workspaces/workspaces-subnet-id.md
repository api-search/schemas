---
description: SubnetId schema from Amazon WorkSpaces API
layout: schema
name: SubnetId
properties_list: []
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-subnet-id-schema.json
slug: workspaces-subnet-id
source_filename: workspaces-subnet-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"^(subnet-([0-9a-f]{8}|[0-9a-f]{17}))$\",\n  \"minLength\": 15,\n  \"maxLength\": 24,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubnetId\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-subnet-id-schema.json\",\n  \"description\": \"SubnetId schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-subnet-id-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: SubnetId
---
