---
description: Avail Configuration
layout: schema
name: AvailConfiguration
properties_list:
- description: ''
  name: AvailSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-avail-configuration-schema.json
slug: medialive-api-avail-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-avail-configuration-schema.json\",\n  \"title\": \"AvailConfiguration\",\n  \"description\": \"Avail Configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availSettings\"\n          },\n          \"description\": \"Controls how SCTE-35 messages create cues. Splice Insert mode treats all segmentation signals traditionally. With Time Signal APOS mode only Time Signal Placement Opportunity and Break messages create segment breaks. With ESAM mode, signals are forwarded to an ESAM server for possible update.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-avail-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvailConfiguration
---
