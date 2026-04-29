---
description: ContainerARN schema from Amazon MediaStore API
layout: schema
name: ContainerARN
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-container-arn-schema.json
slug: mediastore-api-container-arn
source_filename: mediastore-api-container-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-container-arn-schema.json\",\n  \"title\": \"ContainerARN\",\n  \"description\": \"ContainerARN schema from Amazon MediaStore API\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws:mediastore:[a-z]+-[a-z]+-\\\\d:\\\\d{12}:container/[\\\\w-]{1,255}\",\n  \"minLength\": 1,\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-container-arn-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ContainerARN
---
