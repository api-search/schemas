---
description: KeyAliasArn schema from Amazon Ground Station API
layout: schema
name: KeyAliasArn
properties_list: []
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-key-alias-arn-schema.json
slug: ground-station-key-alias-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-key-alias-arn-schema.json\",\n  \"title\": \"KeyAliasArn\",\n  \"description\": \"KeyAliasArn schema from Amazon Ground Station API\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[a-zA-Z-]{0,16}:kms:[a-z]{2}(-[a-z]{1,16}){1,3}-\\\\d{1}:\\\\d{12}:((alias/[a-zA-Z0-9:/_-]{1,256}))$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-key-alias-arn-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: KeyAliasArn
---
