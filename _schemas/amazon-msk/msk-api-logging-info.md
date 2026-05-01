---
description: LoggingInfo schema from Amazon MSK API
layout: schema
name: LoggingInfo
properties_list:
- description: ''
  name: BrokerLogs
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-logging-info-schema.json
slug: msk-api-logging-info
source_filename: msk-api-logging-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-logging-info-schema.json\",\n  \"title\": \"LoggingInfo\",\n  \"description\": \"LoggingInfo schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerLogs\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BrokerLogs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-logging-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: LoggingInfo
---
