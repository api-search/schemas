---
description: ''
layout: schema
name: SiteDeviceAssociation
properties_list:
- description: List of device serial numbers to associate.
  name: device_id
  type: array
- description: Type of devices being associated.
  name: device_type
  type: string
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-site-device-association-schema.json
slug: aruba-central-site-device-association
source_filename: aruba-central-site-device-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SiteDeviceAssociation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"device_id\": {\n      \"type\": \"array\",\n      \"description\": \"List of device serial numbers to associate.\"\n    },\n    \"device_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of devices being associated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-site-device-association-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: SiteDeviceAssociation
---
