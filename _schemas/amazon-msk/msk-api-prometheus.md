---
description: <p>Prometheus settings.</p>
layout: schema
name: Prometheus
properties_list:
- description: ''
  name: JmxExporter
  type: object
- description: ''
  name: NodeExporter
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-prometheus-schema.json
slug: msk-api-prometheus
source_filename: msk-api-prometheus-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-prometheus-schema.json\",\n  \"title\": \"Prometheus\",\n  \"description\": \"\\n            <p>Prometheus settings.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JmxExporter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JmxExporter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"jmxExporter\"\n          },\n          \"description\": \"\\n            <p>Indicates whether you want to turn on or turn off the JMX Exporter.</p>\"\n        }\n      ]\n    },\n    \"NodeExporter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeExporter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nodeExporter\"\n          },\n          \"description\": \"\\n            <p>Indicates whether\
  \ you want to turn on or turn off the Node Exporter.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-prometheus-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Prometheus
---
