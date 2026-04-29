---
description: ContainerStatus schema from Amazon MediaStore API
layout: schema
name: ContainerStatus
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-container-status-schema.json
slug: mediastore-api-container-status
source_filename: mediastore-api-container-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-container-status-schema.json\",\n  \"title\": \"ContainerStatus\",\n  \"description\": \"ContainerStatus schema from Amazon MediaStore API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACTIVE\",\n    \"CREATING\",\n    \"DELETING\"\n  ],\n  \"minLength\": 1,\n  \"maxLength\": 16\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-container-status-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ContainerStatus
---
