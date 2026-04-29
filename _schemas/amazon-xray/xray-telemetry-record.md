---
description: <p/>
layout: schema
name: TelemetryRecord
properties_list:
- description: ''
  name: Timestamp
  type: object
- description: ''
  name: SegmentsReceivedCount
  type: object
- description: ''
  name: SegmentsSentCount
  type: object
- description: ''
  name: SegmentsSpilloverCount
  type: object
- description: ''
  name: SegmentsRejectedCount
  type: object
- description: ''
  name: BackendConnectionErrors
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-telemetry-record-schema.json
slug: xray-telemetry-record
source_filename: xray-telemetry-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Timestamp\"\n  ],\n  \"properties\": {\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"SegmentsReceivedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"SegmentsSentCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"SegmentsSpilloverCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"SegmentsRejectedCount\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"BackendConnectionErrors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackendConnectionErrors\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TelemetryRecord\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-telemetry-record-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-telemetry-record-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: TelemetryRecord
---
