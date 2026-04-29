---
description: Udp Container Settings
layout: schema
name: UdpContainerSettings
properties_list:
- description: ''
  name: M2tsSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-udp-container-settings-schema.json
slug: medialive-api-udp-container-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-udp-container-settings-schema.json\",\n  \"title\": \"UdpContainerSettings\",\n  \"description\": \"Udp Container Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"M2tsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"m2tsSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-udp-container-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UdpContainerSettings
---
