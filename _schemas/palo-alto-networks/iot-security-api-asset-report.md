---
description: AssetReport schema from Palo Alto Networks IoT Security API
layout: schema
name: AssetReport
properties_list:
- description: Total number of discovered devices.
  name: total_devices
  type: integer
- description: Number of actively monitored devices.
  name: monitored_devices
  type: integer
- description: Device count breakdown by category.
  name: by_category
  type: object
- description: Device count breakdown by risk level.
  name: by_risk_level
  type: object
- description: Device count breakdown by network site.
  name: by_site
  type: array
- description: Most common device profiles.
  name: top_profiles
  type: array
- description: Timestamp when the report was generated.
  name: report_time
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/iot-security-api-asset-report-schema.json
slug: iot-security-api-asset-report
source_filename: iot-security-api-asset-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetReport\",\n  \"description\": \"AssetReport schema from Palo Alto Networks IoT Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-asset-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_devices\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of discovered devices.\"\n    },\n    \"monitored_devices\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of actively monitored devices.\"\n    },\n    \"by_category\": {\n      \"type\": \"object\",\n      \"description\": \"Device count breakdown by category.\",\n      \"additionalProperties\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"by_risk_level\": {\n      \"type\": \"object\",\n      \"description\": \"Device count breakdown by risk level.\",\n      \"properties\"\
  : {\n        \"critical\": {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"by_site\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"site\": {\n            \"type\": \"string\"\n          },\n          \"device_count\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"Device count breakdown by network site.\"\n    },\n    \"top_profiles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"profile\": {\n            \"type\": \"string\"\n          },\n          \"device_count\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"Most common\
  \ device profiles.\"\n    },\n    \"report_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the report was generated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-asset-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AssetReport
---
