---
description: <p>Indicates whether you want to turn on or turn off the Node Exporter.</p>
layout: schema
name: NodeExporterInfo
properties_list:
- description: ''
  name: EnabledInBroker
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-node-exporter-info-schema.json
slug: msk-api-node-exporter-info
source_filename: msk-api-node-exporter-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-node-exporter-info-schema.json\",\n  \"title\": \"NodeExporterInfo\",\n  \"description\": \"\\n            <p>Indicates whether you want to turn on or turn off the Node Exporter.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EnabledInBroker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabledInBroker\"\n          },\n          \"description\": \"\\n            <p>Indicates whether you want to turn on or turn off the Node Exporter.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EnabledInBroker\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-node-exporter-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NodeExporterInfo
---
