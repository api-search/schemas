---
description: A single IP address or an IP address range in CIDR notation
layout: schema
name: IpRange
properties_list: []
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-ip-range-schema.json
slug: workspaces-web-ip-range
source_filename: workspaces-web-ip-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"^\\\\d{1,3}\\\\.\\\\d{1,3}\\\\.\\\\d{1,3}\\\\.\\\\d{1,3}(?:/([0-9]|[12][0-9]|3[0-2])|)$\",\n  \"description\": \"A single IP address or an IP address range in CIDR notation\",\n  \"format\": \"password\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IpRange\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-range-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-range-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: IpRange
---
