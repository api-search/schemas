---
description: the option to configure log subscription.
layout: schema
name: ConfigureLogsRequest
properties_list:
- description: ''
  name: EgressAccessLogs
  type: object
- description: ''
  name: IngressAccessLogs
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-configure-logs-request-schema.json
slug: mediapackage-api-configure-logs-request
source_filename: mediapackage-api-configure-logs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-configure-logs-request-schema.json\",\n  \"title\": \"ConfigureLogsRequest\",\n  \"description\": \"the option to configure log subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressAccessLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EgressAccessLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressAccessLogs\"\n          }\n        }\n      ]\n    },\n    \"IngressAccessLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IngressAccessLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingressAccessLogs\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-configure-logs-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigureLogsRequest
---
