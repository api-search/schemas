---
description: LogDestinationType schema from Amazon Network Firewall
layout: schema
name: LogDestinationType
properties_list: []
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-log-destination-type-schema.json
slug: openapi-log-destination-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-log-destination-type-schema.json\",\n  \"title\": \"LogDestinationType\",\n  \"description\": \"LogDestinationType schema from Amazon Network Firewall\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"S3\",\n    \"CloudWatchLogs\",\n    \"KinesisDataFirehose\"\n  ],\n  \"pattern\": \"[0-9A-Za-z]+\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-log-destination-type-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: LogDestinationType
---
