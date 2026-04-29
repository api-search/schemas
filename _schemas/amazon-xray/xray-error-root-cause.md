---
description: The root cause of a trace summary error.
layout: schema
name: ErrorRootCause
properties_list:
- description: ''
  name: Services
  type: object
- description: ''
  name: ClientImpacting
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-error-root-cause-schema.json
slug: xray-error-root-cause
source_filename: xray-error-root-cause-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorRootCauseServices\"\n        },\n        {\n          \"description\": \"A list of services corresponding to an error. A service identifies a segment and it contains a name, account ID, type, and inferred flag.\"\n        }\n      ]\n    },\n    \"ClientImpacting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"A flag that denotes that the root cause impacts the trace client.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The root cause of a trace summary error.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorRootCause\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-error-root-cause-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-error-root-cause-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ErrorRootCause
---
