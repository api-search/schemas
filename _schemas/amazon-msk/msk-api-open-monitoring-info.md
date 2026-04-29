---
description: <p>JMX and Node monitoring for the MSK cluster.</p>
layout: schema
name: OpenMonitoringInfo
properties_list:
- description: ''
  name: Prometheus
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-open-monitoring-info-schema.json
slug: msk-api-open-monitoring-info
source_filename: msk-api-open-monitoring-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-open-monitoring-info-schema.json\",\n  \"title\": \"OpenMonitoringInfo\",\n  \"description\": \"\\n            <p>JMX and Node monitoring for the MSK cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prometheus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrometheusInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"prometheus\"\n          },\n          \"description\": \"\\n            <p>Prometheus settings.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Prometheus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-open-monitoring-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OpenMonitoringInfo
---
