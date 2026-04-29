---
description: S3KeyPrefix schema from Amazon Ground Station API
layout: schema
name: S3KeyPrefix
properties_list: []
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-s3-key-prefix-schema.json
slug: ground-station-s3-key-prefix
source_filename: ground-station-s3-key-prefix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-key-prefix-schema.json\",\n  \"title\": \"S3KeyPrefix\",\n  \"description\": \"S3KeyPrefix schema from Amazon Ground Station API\",\n  \"type\": \"string\",\n  \"pattern\": \"^([a-zA-Z0-9_\\\\-=/]|\\\\{satellite_id\\\\}|\\\\{config\\\\-name}|\\\\{s3\\\\-config-id}|\\\\{year\\\\}|\\\\{month\\\\}|\\\\{day\\\\}){1,900}$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-s3-key-prefix-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: S3KeyPrefix
---
