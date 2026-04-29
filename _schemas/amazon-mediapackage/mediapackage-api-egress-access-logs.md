---
description: Configure egress access logging.
layout: schema
name: EgressAccessLogs
properties_list:
- description: ''
  name: LogGroupName
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-egress-access-logs-schema.json
slug: mediapackage-api-egress-access-logs
source_filename: mediapackage-api-egress-access-logs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-egress-access-logs-schema.json\",\n  \"title\": \"EgressAccessLogs\",\n  \"description\": \"Configure egress access logging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logGroupName\"\n          },\n          \"description\": \"Customize the log group name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-egress-access-logs-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: EgressAccessLogs
---
