---
description: IpV4AddressList schema
layout: schema
name: IpV4AddressList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-ip-v4-address-list-schema.json
slug: inspector-ip-v4-address-list
source_filename: inspector-ip-v4-address-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ip-v4-address-list-schema.json\",\n  \"title\": \"IpV4AddressList\",\n  \"description\": \"IpV4AddressList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\\\\.){3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$\",\n    \"minLength\": 7,\n    \"maxLength\": 15\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ip-v4-address-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: IpV4AddressList
---
