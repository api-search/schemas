---
description: TagMapUpdate schema
layout: schema
name: TagMapUpdate
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-tag-map-update-schema.json
slug: incident-manager-tag-map-update
source_filename: incident-manager-tag-map-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-tag-map-update-schema.json\",\n  \"title\": \"TagMapUpdate\",\n  \"description\": \"TagMapUpdate schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"string\",\n    \"pattern\": \"^[A-Za-z0-9 _=@:.+-/]*$\",\n    \"minLength\": 0,\n    \"maxLength\": 256\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-tag-map-update-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: TagMapUpdate
---
